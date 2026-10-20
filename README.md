# Wordle

A customizable Wordle-style iOS game built with Swift and UIKit. Choose a word length, set your guess limit, select a word theme, and try to solve the hidden word.

## Features

- Choose a target word length from 4 to 7 letters.
- Set the number of guesses from 3 to 8.
- Choose the Normal, Animals, or Countries word theme.
- Enable Alien Wordle to change the target after each submitted guess.
- Get color-coded feedback on each guess:
  - Green: correct letter in the correct position.
  - Yellow: letter is in the word, but in a different position.
  - Gray: letter is not in the target word.
- Reset the board while keeping the current settings.

## Requirements

- Xcode
- iOS 16.1 or later

The project uses Swift and UIKit and has no third-party package dependencies.

## Run the app

1. Clone or download this repository.
2. Open `Wordle.xcodeproj` in Xcode.
3. Select the **Wordle** scheme and an iOS Simulator or connected device.
4. Build and run the app with **Product → Run** (`⌘R`).

To run on a physical device, configure code signing with your Apple development team in Xcode.

## How to play

1. Enter a guess using the on-screen keyboard. Use the delete key to remove a letter.
2. Submit a complete row to see feedback for your guess.
3. Use the feedback to solve the target before you run out of guesses.
4. Open **Settings** to change the word length, guess limit, theme, or Alien Wordle mode. Applying new settings starts a new board.

In Alien Wordle mode, the target changes after each submitted row, so feedback does not carry over to the next guess.

## Tests

The project includes unit and UI test targets. Run the tests in Xcode with **Product → Test** (`⌘U`).

## Project structure

- `Wordle/` — app source code, storyboards, and assets.
- `WordleTests/` — unit tests.
- `WordleUITests/` — UI tests.
- `Wordle.xcodeproj/` — Xcode project.

## Note

The game uses a small built-in word list rather than a full dictionary.
