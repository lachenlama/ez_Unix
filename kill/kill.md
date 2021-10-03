# Kill command
- kill command in Linux (located in /bin/kill), is a built-in command which is used to terminate processes manually. kill command sends a signal to a process which terminates the process. If the user doesn’t specify any signal which is to be sent along with kill command then default TERM signal is sent that terminates the process.

# Options and examples
1. kill -l :To display all the available signals you can use below command option:
- Syntax: $kill -l

2. kill pid : To show how to use a PID with the kill command.
- Syntax: $kill pid

3. kill -s : To show how to send signal to processes.
- Syntax: kill {-signal | -s signal} pid 

4. kill -L :This command is used to list available signals in a table format.
- Syntax: kill {-l | --list[=signal] | -L | --table} 