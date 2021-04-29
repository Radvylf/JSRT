# JSRT

JavaScript Rudimentary Terminal: A basic I/O and storage API

## Installation

To use JSRT, download the latest JSRT.html. Any of your JS files should be added under `<!-- Your JS Files -->` (near the end of the file).

In order to run some code once JSRT is loaded, you can put a function in `JSRT.onload`.

## Usage

In browsers where ES6 are supported, `JSRT.terminal` will contain asynchronous versions of all functions (where asynchronous operations occur). The `JSRT.old_terminal` object has all of the same features, but asynchronous operations (mainly input) will take callbacks instead.

**`JSRT.terminal` and `JSRT.old_terminal`:**

- `print`: Print a string to the terminal, followed by a `\n`
- `write`: Print a string to the terminal, without a `\n`
- `backspace`: Remove the last character in the terminal (if `\n`, do nothing)
- `carriage_return`: Remove the last line in the terminal
- `blank`: Clear the terminal
- `title`: Get the current title (initially the empty string)
- `write_title`: Sets the title
- `input_r`: Input a character from the keyboard
- `input_d`: Input a keystroke from the keyboard: a UTF-8 code point, followed by flags for meta, alt, and ctrl
- `input_p`: Input a line of text from the user
- `store`: Store something in local storage
- `retrieve`: Retrieve something from local storage

The terminal takes input in a very rudimentary way. It is not very accessible, and you cannot move or see the cursor.
