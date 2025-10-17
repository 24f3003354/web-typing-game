# TypeLite — Minimal Monkeytype-like Typing Game

MIT-licensed, zero-dependency, dark-themed typing test inspired by Monkeytype. Runs entirely in your browser with a clean UI, live WPM/accuracy stats, and multiple time limits.

## Overview

TypeLite is a minimal typing game that:
- Displays a stream of words in a dark, distraction-free interface
- Starts on first keypress, with a blinking caret and current-word highlight
- Tracks WPM and accuracy live during the test
- Supports time limits: 30s, 60s, 120s
- Allows correcting within the current word using Backspace
- Lets you restart quickly with Tab or the Restart button

Built with plain HTML, CSS, and JavaScript — no frameworks required.

## Setup

No build step needed.

- Option 1: Open index.html directly in your browser.
- Option 2: Serve locally (recommended for best behavior across browsers):
  - Python 3: python -m http.server 8080
  - Node (serve): npx serve .
  - Bun: bunx serve .

Then open http://localhost:8080 in your browser.

## Usage

- Click the words area to focus (mobile: this brings up the keyboard).
- Start typing; the timer begins on your first keypress.
- Use Space to move to the next word.
- Use Backspace to correct within the current word.
- Press Tab or click Restart to reset the test.
- Change the time limit via the segmented control (resets the test).

Stats:
- WPM: Calculated as correct characters / 5 over elapsed minutes.
- Accuracy: Correct characters divided by all typed characters.

Keyboard shortcuts:
- Tab: Restart
- Enter: Restart when a test has ended

Note: For simplicity, backspacing into a previous word is disabled in this minimal version.

## License

MIT License

Copyright (c) 2025 TypeLite contributors

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the “Software”), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.