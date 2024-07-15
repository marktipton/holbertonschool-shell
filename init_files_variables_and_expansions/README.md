# Shell Scripting and Environment Variables

## Learning Objectives

### General

- **What happens when you type `$ ls -l *.txt`?**
  - The shell expands `*.txt` to match all `.txt` files in the current directory, then `ls -l` lists these files in long format.

### Shell Initialization Files

- **Files and Directories**
  - **`/etc/profile`**: A script that runs at login for all users.
  - **`/etc/profile.d`**: A directory containing scripts that are sourced by `/etc/profile`.
  - **`~/.bashrc`**: A script that runs for non-login interactive shells.

### Variables

- **Types of Variables**
  - **Local Variable**: Only available within the current shell session.
  - **Global Variable**: Available to the current shell and any child processes.

- **Reserved Variables**
  - Special variables predefined by the shell, such as `HOME`, `PATH`, `PS1`.

- **Creating, Updating, and Deleting Variables**
  - **Create/Update**: `VAR=value`
  - **Delete**: `unset VAR`

- **Roles of Reserved Variables**
  - **`HOME`**: The home directory of the current user.
  - **`PATH`**: The directories to search for executable files.
  - **`PS1`**: The primary prompt string.

- **Special Parameters**
  - **`$?`**: The exit status of the last command executed.

### Expansions

- **What is Expansion?**
  - The process of substituting values or performing operations before command execution.

- **Quotes**
  - **Single Quotes (`'`)**: Preserve the literal value of each character enclosed.
  - **Double Quotes (`"`)**: Allow variable and command substitution within the enclosed text.

- **Command Substitution**
  - **Using `$()`**: `$(command)`
  - **Using Backticks**: `` `command` ``

### Shell Arithmetic

- **Performing Arithmetic Operations**
  - Use the `$((expression))` syntax for arithmetic calculations.

### The `alias` Command

- **Creating an Alias**
  - `alias name='command'`

- **Listing Aliases**
  - `alias`

- **Temporarily Disabling an Alias**
  - Use a backslash before the command: `\command`

### Other Help Pages

- **Commands**
  - **`printenv`**: Print all or part of environment variables.
  - **`set`**: Set or unset shell options and positional parameters.
  - **`unset`**: Unset values and attributes of shell variables and functions.
  - **`export`**: Set the export attribute for shell variables.
  - **`alias`**: Define or display aliases.
  - **`unalias`**: Remove alias definitions.
  - **`.` (dot command)**: Source a file in the current shell.
  - **`source`**: Source a file in the current shell (same as `.`).
  - **`printf`**: Format and print data.

- **Executing Commands from a File**
  - Use `. filename` or `source filename` to execute commands from a file in the current shell.

## Requirements

### General

- **Allowed editors**: vi, vim, emacs
- **Scripts tested on**: Ubuntu 20.04 LTS
- **Script constraints**:
  - Exactly two lines long (`wc -l file` should print 2)
  - End with a new line
  - First line should be `#!/bin/bash`
  - Include a `README.md` file in the project folder describing each script
  - Scripts must be executable (`chmod u+x file`)
  - **Prohibited**: backticks, `&&`, `||`, `;`, `sed`, `awk`

## Common Commands

- `printenv`: Print all or part of environment variables
- `set`: Set or unset shell options and positional parameters
- `unset`: Unset values and attributes of shell variables and functions
- `export`: Set the export attribute for shell variables
- `alias`: Define or display aliases
- `unalias`: Remove alias definitions
- `.`: Source a file in the current shell
- `source`: Source a file in the current shell (same as `.`)
- `printf`: Format and print data
