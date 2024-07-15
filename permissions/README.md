# User and File Permissions Management

## Learning Objectives

### Permissions

- **Commands and Their Functions**
  - **`chmod`**: Change the permissions of a file or directory
  - **`sudo`**: Execute a command as another user, typically the superuser
  - **`su`**: Switch user or become superuser
  - **`chown`**: Change the owner of a file or directory
  - **`chgrp`**: Change the group ownership of a file or directory
  - **`id`**: Print user and group IDs
  - **`groups`**: Print the groups a user is a member of
  - **`whoami`**: Print the current user name
  - **`adduser`**: Add a user to the system (Debian-based systems)
  - **`useradd`**: Add a user to the system (more universal, lower-level command)
  - **`addgroup`**: Add a group to the system

### Linux File Permissions

- **Representation of Permissions**
  - **Three Sets of Permissions**:
    - **Owner**: The user who owns the file
    - **Group**: Users who are members of the file’s group
    - **Other**: All other users

  - **Permission Types**:
    - **Read (r)**: 4
    - **Write (w)**: 2
    - **Execute (x)**: 1

  - **Combining Permissions**:
    - Permissions are represented by combining the digits for each set. For example:
      - `rwx` (7) for read, write, and execute
      - `r-x` (5) for read and execute
      - `rw-` (6) for read and write

- **Changing Permissions, Owner, and Group**
  - **Change Permissions**:
    - Syntax: `chmod [options] mode file`
    - Example: `chmod 755 file` (owner can read/write/execute, others can read/execute)
  - **Change Owner**:
    - Syntax: `chown [options] owner file`
    - Example: `sudo chown user file`
  - **Change Group**:
    - Syntax: `chgrp [options] group file`
    - Example: `sudo chgrp group file`

- **Why Normal Users Cannot Use `chown`**
  - Changing file ownership can affect system security and integrity. Only the superuser (root) can change file ownership.

- **Running Commands with Root Privileges**
  - Use `sudo` before a command to run it with superuser privileges.
  - Example: `sudo command`

- **Changing User ID or Becoming Superuser**
  - **Change User ID**: `su - username`
  - **Become Superuser**: `su` (switch to root)
