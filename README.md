# ez Unix : Learn Unix the ez way.

Celebrate [Hacktoberfest](https://hacktoberfest.digitalocean.com/) by getting involved in the open source community by completing some simple tasks in this project. 

## Repository's Aim
* The repository is for Unix commands and their uses. The contributors may add what they wish within the context of being used in Unix Cli. 
* We recommend the contributors to use Cli to clone, write code and push your code to this repository.
* Please mention the command and also its uses by making a dir itself in the repository :
    * for instance, if "ls" is the command you are committing then name the directory file "ls" and writes the commands function as a .txt file inside the directory. Add a screenshot of the command and its output if needed.
* Also add the command in the "Commands" section of "README.md" file below. 
* Other than that, the contributors are free to issue a PR with anything related to Cli in this repository.

## Commands
<!-- Add your contributed command down below :- -->
- ls
- kill
## description
- kill command in Linux (located in /bin/kill), is a built-in command which is used to terminate processes manually. kill command sends a signal to a process which terminates the process. If the user doesn’t specify any signal which is to be sent along with kill command then default TERM signal is sent that terminates the process.
### Options and examples
- 1. kill -l :To display all the available signals you can use below command option:
- Syntax: $kill -l
- 2. kill pid : To show how to use a PID with the kill command.
- Syntax: $kill pid
- 3.  kill -s : To show how to send signal to processes.
- Syntax: kill {-signal | -s signal} pid 
- 4. kill -L :This command is used to list available signals in a table format.
- Syntax: kill {-l | --list[=signal] | -L | --table} 


