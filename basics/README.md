# Shell and Command Line Basics

## Learning Objectives

### General

- **What does RTFM mean?**
  - RTFM stands for "Read The _____ Manual." A lot of questions can be answered by just consulting the documentation. 

- **What is a Shebang?**
  - A shebang (`#!`) is a character sequence at the beginning of a script that specifies the interpreter to be used to execute the script.

- **What is the Shell?**
  - The shell is a command-line interface that allows users to interact with the operating system by typing commands.

- **What is the difference between a terminal and a shell?**
  - The terminal is the interface that displays the shell and allows user input, while the shell is the program that processes commands.

- **What is the shell prompt?**
  - The shell prompt is a symbol or series of characters indicating the shell is ready to accept commands.

- **How to use the history (the basics)**
  - The history command lists previously executed commands, allowing users to reuse or modify them.

### Navigation

- **Commands and Built-ins**
  - `cd`: Change directory
  - `pwd`: Print working directory
  - `ls`: List directory contents

- **Filesystem Navigation**
  - The `.` directory refers to the current directory.
  - The `..` directory refers to the parent directory.
  - The working directory is the current directory in which the user is operating. Use `pwd` to print it and `cd` to change it.
  - The root directory is the top level of the filesystem.
  - The home directory is the default directory for a user. Use `cd` to navigate to it.
  - The root directory is `/` while the root user's home directory is `/root`.

- **Hidden Files**
  - Hidden files start with a `.` and can be listed with `ls -a`.

- **Command: `cd -`**
  - `cd -` switches to the previous directory.

### Looking Around

- **Commands**
  - `ls`: List directory contents
  - `less`: View file contents
  - `file`: Determine file type

- **Using Options and Arguments**
  - Commands can take options (preceded by `-`) and arguments to modify their behavior.

- **`ls` Long Format**
  - Use `ls -l` to display detailed information about files and directories.

### A Guided Tour

- **Commands**
  - `ln`: Create links between files

- **Common Directories**
  - Typical directories include `/bin`, `/etc`, `/home`, `/usr`, etc.

- **Links**
  - Symbolic link: Points to another file or directory.
  - Hard link: Direct reference to the file's data on disk.
  - Differences: Symbolic links can span filesystems and reference directories, hard links cannot.

### Manipulating Files

- **Commands**
  - `cp`: Copy files or directories
  - `mv`: Move or rename files or directories
  - `rm`: Remove files or directories
  - `mkdir`: Create directories

- **Wildcards**
  - Wildcards (`*`, `?`, `[]`) match multiple files or patterns.

### Working with Commands

- **Commands**
  - `type`: Display information about command type
  - `which`: Locate a command
  - `help`: Display help for built-in commands
  - `man`: Display manual pages

- **Command Types**
  - Shell built-ins, aliases, functions, and external commands.

- **Aliases**
  - Custom shortcuts for commands.

- **`help` vs `man`**
  - `help` is used for shell built-ins, while `man` provides detailed manual pages.

### Reading Man Pages

- **Sections**
  - User commands (1), System calls (2), Library functions (3).

### Keyboard Shortcuts for Bash

- **Common Shortcuts**
  - Examples: `Ctrl+C` to cancel a command, `Ctrl+R` to search command history.

### LTS

- **What does LTS mean?**
  - LTS stands for Long-Term Support, indicating a version with extended support and maintenance.

## Requirements

### General

- **Allowed editors**: vi, vim, emacs
- **Scripts tested on**: Ubuntu 22.04 LTS
- **Script constraints**:
  - Exactly two lines long (`wc -l file` should print 2)
  - End with a new line
  - First line should be `#!/bin/bash`
  - Include a `README.md` file in the repo and project folder
  - Scripts must be executable (`chmod u+x file`)
- **Prohibited**: backticks, `&&`, `||`, `;`

## Common Commands

- `cd`: Change directory
- `ls`: List directory contents
- `pwd`: Print working directory
- `less`: View file contents
- `file`: Determine file type
- `ln`: Create links between files
- `cp`: Copy files or directories
- `mv`: Move or rename files or directories
- `rm`: Remove files or directories
- `mkdir`: Create directories
- `type`: Display information about command type
- `which`: Locate a command
- `help`: Display help for built-in commands
- `man`: Display manual pages
