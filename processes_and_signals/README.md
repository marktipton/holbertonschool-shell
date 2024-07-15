# Process Management and Signals

## Learning Objectives

### General

- **What is a PID?**
  - A PID (Process ID) is a unique identifier assigned by the operating system to each process when it is created.

- **What is a Process?**
  - A process is an instance of a program that is being executed. It contains the program code and its current activity.

- **How to Find a Process’ PID**
  - Use the `ps` command to list processes and their PIDs.
  - Use `pgrep` followed by the process name to find its PID.

- **How to Kill a Process**
  - Use the `kill` command followed by the PID to terminate a process.
  - Use `pkill` followed by the process name to kill all processes matching the name.

### Signals

- **What is a Signal?**
  - A signal is a limited form of inter-process communication used in Unix, Unix-like, and other POSIX-compliant operating systems. It is used to notify a process that a particular event has occurred.

- **Signals that Cannot Be Ignored**
  - **SIGKILL (9)**: Immediately terminates the process. Cannot be caught, blocked, or ignored.
  - **SIGSTOP (19)**: Stops (pauses) the process execution. Cannot be caught, blocked, or ignored.

## Common Commands

- **`ps`**: Report a snapshot of current processes.
  - Example: `ps aux`

- **`pgrep`**: Look up processes based on name and other attributes.
  - Example: `pgrep process_name`

- **`pkill`**: Send signals to processes based on name and other attributes.
  - Example: `pkill process_name`

- **`kill`**: Send a signal to a process.
  - Example: `kill -SIGKILL PID`

- **`exit`**: Exit the shell or a shell script.
  - Example: `exit 0`

- **`trap`**: Define and activate handlers to run when the shell receives signals.
  - Example: `trap 'commands' SIGNAL`
