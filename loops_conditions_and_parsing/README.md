# Shell Scripting and Control Structures

## Learning Objectives

### General

- **Advantage of Using `#!/usr/bin/env bash` Over `#!/bin/bash`**
  - `#!/usr/bin/env bash` is more portable as it locates the `bash` executable using the `env` command, ensuring the script works even if `bash` is not in the usual location (`/bin/bash`).

- **Loops in Shell Scripting**
  - **`while` Loop**
    - Syntax:
      ```bash
      while [ condition ]; do
        # commands
      done
      ```
  - **`until` Loop**
    - Syntax:
      ```bash
      until [ condition ]; do
        # commands
      done
      ```
  - **`for` Loop**
    - Syntax:
      ```bash
      for variable in list; do
        # commands
      done
      ```

- **Conditional Statements**
  - **`if`, `else`, `elif`**
    - Syntax:
      ```bash
      if [ condition ]; then
        # commands
      elif [ condition ]; then
        # commands
      else
        # commands
      fi
      ```
  - **`case` Statement**
    - Syntax:
      ```bash
      case value in
        pattern1)
          # commands
          ;;
        pattern2)
          # commands
          ;;
        *)
          # default commands
          ;;
      esac
      ```

- **Using the `cut` Command**
  - **Function**: Remove sections from each line of files.
  - **Syntax**: 
    ```bash
    cut [options] [file]
    ```
  - **Common Options**:
    - `-d` : Define a delimiter
    - `-f` : Specify fields to extract

- **File and Comparison Operators**
  - **File Operators**
    - `-e` : Check if a file exists
    - `-f` : Check if it is a regular file
    - `-d` : Check if it is a directory
  - **Comparison Operators**
    - **String Comparison**
      - `=` : Equal
      - `!=` : Not equal
    - **Numeric Comparison**
      - `-eq` : Equal
      - `-ne` : Not equal
      - `-lt` : Less than
      - `-le` : Less than or equal
      - `-gt` : Greater than
      - `-ge` : Greater than or equal

## Requirements

### General

- **Allowed editors**: vi, vim, emacs
- **Scripts tested on**: Ubuntu 20.04 LTS
- **Script constraints**:
  - Exactly two lines long (`wc -l file` should print 2)
  - End with a new line
  - First line should be `#!/usr/bin/env bash`
  - Include a `README.md` file in the project folder describing each script
  - Scripts must be executable (`chmod u+x file`)
  - **Prohibited**: backticks, `&&`, `||`, `;`, `sed`, `awk`

## Common Commands

- `env`: Display and modify the environment
- `cut`: Remove sections from each line of files
- `for`: Iterate over a list of items
- `while`: Execute commands as long as a condition is true
- `until`: Execute commands until a condition becomes true
- `if`: Conditional execution
