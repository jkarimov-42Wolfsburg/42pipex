# 42cursus - pipex

Implementing Pipex in C involves understanding how to manage processes, file descriptors, and pipes. Here's a brief outline of what you need to learn:


**Processes and fork():** 

Understand how to create child processes using fork(). Each process has its own address space, so modifications made in one process do not affect the other.


**Executing Commands:**

Learn how to execute commands in C using functions like execvp() or execve(). These functions replace the current process with a new one specified by the command.
Understand how to use these functions to execute commands in the child process after forking.


**Pipes (pipe()):**

Learn how to create pipes using the pipe() system call. Pipes allow inter-process communication by providing a channel for one process to send data to another.
Understand how to create pipes before forking, so both the parent and child processes have access to them.


**File Descriptors:**

File descriptors are used to represent open files, pipes, sockets, etc., in Unix-like operating systems.
Learn how to manipulate file descriptors using functions like dup2() to redirect input and output streams.
Understand how to close unused file descriptors to prevent resource leaks.


**Managing Input and Output:**

Implement logic to handle input and output redirection. This involves using dup2() to redirect standard input and output streams to pipes or files.
Understand how to open and close files as needed.


**Error Handling:
**
Implement error handling to deal with failures in system calls like fork(), pipe(), execvp(), etc.
Learn how to use functions like perror() and fprintf(stderr, ...) to output error messages.


**Argument Parsing:**

Understand how to parse command-line arguments to get the command and arguments for execution.


**Memory Management:**

Learn how to manage memory properly, especially when dealing with dynamically allocated memory.


**Execution Flow:**

Understand the flow of execution in your program, including when to fork, when to execute commands, when to close file descriptors, and when to wait for child processes to finish.

