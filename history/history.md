# History

`history` command is used to view the previously executed commands

```bash
user@user:~$ history
  226  g++ WIPL.cpp 
  227  ./a.out 
  228  g++ WIPL.cpp 
  229  ./a.out 
  230  g++ WIPL.cpp
```

- `history <num>`
    - To see limited number of commands that executed previously
    
    ```bash
    user@user:~$ history 5
     1222  man firefox 
     1223  free -h
     1224  man history
     1225  history
     1226  history 5
    user@user:~$
    ```
    
- Every command executed is treated as an event and has a number associated with it
    - Using event number to execute command
    
    ```bash
    user@user:~$ history 5
     1222  man firefox 
     1223  free -h
     1224  man history
     1225  history
     1226  history 5
    user@user:~$ !1223
    free -h
                  total        used        free      shared  buff/cache   available
    Mem:          7.6Gi       1.8Gi       343Mi       564Mi       5.5Gi       5.0Gi
    Swap:         2.0Gi       128Mi       1.9Gi
    user@user:~$
    ```
    
    - `:p` To view the command associated with the event number
    
    ```bash
    user@user:~$ !1223:p
    free -h
    user@user:~$ !12223:p
    bash: !12223: event not found
    user@user:~$
    ```
    
    - To execute a command without being stored in the history
    
    ```bash
    user@user:~$ echo $HISTFILE
    /home/user/.bash_history
    user@user:~$ unset HISTFILE
    user@user:~$ echo $HISTFILE
    
    user@user:~$
    ```
    
    - To remove history
        - `history -d event_number to remove one event`
        - `history -c to remove whole history`
