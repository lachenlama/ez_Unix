
# ps

## Overview
As is a multitasking and multi-user systems it runs the multiple process at same time. So to list the current running process we have command "ps" (abbreviation for Process Status) Command "ps" list the current running process with PID and Other realted Infoamtion. Its uses /proc file to get this information. 

## Syntax
```
ps [options]
```

## Demo
```
[root@ars ~]# ps
  PID TTY          TIME CMD
12330 pts/0    00:00:00 bash
21621 pts/0    00:00:00 ps
```

Where:
* PID – the unique process ID
* TTY – terminal type that the user is logged into
* TIME – amount of CPU in minutes and seconds that the process has been running
* CMD – name of the command that launched the process.
