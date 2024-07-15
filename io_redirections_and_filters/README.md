# Shell Commands and I/O Redirection

## Learning Objectives

### Shell, I/O Redirection

- **Commands and Their Functions**
  - `head`: Output the first part of files
  - `tail`: Output the last part of files
  - `find`: Search for files in a directory hierarchy
  - `wc`: Print newline, word, and byte counts for each file
  - `sort`: Sort lines of text files
  - `uniq`: Report or omit repeated lines
  - `grep`: Print lines matching a pattern
  - `tr`: Translate or delete characters
  - `echo`: Display a line of text
  - `cat`: Concatenate files and print on the standard output
  - `rev`: Reverse lines characterwise
  - `cut`: Remove sections from each line of files
  - `passwd (5)`: Information about the `/etc/passwd` file format

- **I/O Redirection**
  - **Redirect Standard Output to a File**
    - Use `>` to redirect output to a file (e.g., `command > file`).
  - **Get Standard Input from a File**
    - Use `<` to redirect input from a file (e.g., `command < file`).
  - **Send Output from One Program to Another**
    - Use `|` to pipe output from one command to another (e.g., `command1 | command2`).
  - **Combine Commands and Filters with Redirections**
    - Use a combination of `>`, `<`, and `|` to chain commands and manage I/O.

### Special Characters

- **Common Special Characters and Their Uses**
  - **Whitespace**: Used to separate commands and arguments.
  - **Single Quotes (`'`)**: Preserve the literal value of each character enclosed.
  - **Double Quotes (`"`)**: Preserve the literal value of most characters enclosed, allowing variable expansion.
  - **Backslash (`\`)**: Escape character, used to preserve the literal value of the next character.
  - **Comment (`#`)**: Used to add comments in scripts.
  - **Pipe (`|`)**: Used to pass the output of one command as input to another.
  - **Command Separator (`;`)**: Used to separate multiple commands on a single line.
  - **Tilde (`~`)**: Represents the home directory of the current user.

### Other Man Pages

- **Commands**
  - **`echo`**: Display a line of text.
  - **`cat`**: Concatenate files and print on the standard output.
  - **`rev`**: Reverse lines characterwise.
  - **`cut`**: Remove sections from each line of files.
  - **`passwd (5)`**: Information about the `/etc/passwd` file format.
  - **`shadow (5)`**: Information about the `/etc/shadow` file format.

## Common Commands

- `echo`: Display a line of text
- `cat`: Concatenate files and print on the standard output
- `head`: Output the first part of files
- `tail`: Output the last part of files
- `find`: Search for files in a directory hierarchy
- `wc`: Print newline, word, and byte counts for each file
- `sort`: Sort lines of text files
- `uniq`: Report or omit repeated lines
- `grep`: Print lines matching a pattern
- `tr`: Translate or delete characters
- `rev`: Reverse lines characterwise
- `cut`: Remove sections from each line of files
- `passwd (5)`: Information about the `/etc/passwd` file format
- `shadow (5)`: Information about the `/etc/shadow` file format
