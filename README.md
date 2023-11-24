# Minitalk

## Overview
`Minitalk` is a communication program in the form of a client and server. In this project, students at 42 school learn about UNIX signals and inter-process communication. The client sends a message to the server, which it then displays.

## Features
- Client-server communication using UNIX signals.
- Efficient message transmission using `SIGUSR1` and `SIGUSR2`.
- Bonus part includes support for Unicode characters and a more efficient communication protocol.

## Compilation and Usage
### Requirements
- GCC compiler
- GNU make
- `libftprintf.a` library (included)

### Compiling the Program
To compile both the server and client programs, run:

```
make all
```

This compiles the `server` and `client` executables.

### Compiling the Bonus Program
For the bonus part, which supports Unicode and has an improved protocol:

```
make bonus
```

This compiles the `server_bonus` and `client_bonus` executables.

### Running the Programs
- To start the server, run: `./server`. It will display its PID.
- To send a message from the client, run: `./client [server PID] [message]`.

### Cleaning Up
To clean up compiled files:

```
make fclean
```

To recompile:

```
make re
```

## File Structure
- `src/*.c` - Source files for the standard version.
- `bonus/src/*.c` - Source files for the bonus version.

Enjoy using Minitalk for your basic communication needs!
