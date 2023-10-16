 ## 'netstat' command displays various network related information such as network connections, routing tables, interface statistics, masquerade connections, multicast memberships etc.

 - To show both listening and non-listening sockets.

 ```bash
    netstat -a
 ```

 - To list all tcp ports.

 ```bash
    netstat -at
 ```

 - To list all udp ports.

 ```bash
    netstat -au
 ```

 - To list only the listening ports.

 ```bash
    netstat -l
 ```