Reports file system disk usage

```bash
user@user:~$ df
Filesystem     1K-blocks     Used Available Use% Mounted on
udev             3977808        0   3977808   0% /dev
tmpfs             801396     2432    798964   1% /run
/dev/sda7      154274224 20535716 125832156  15% /
```

device name, total blocks, used disk space , available disk space and mount points on the file system.

- df -a( —all)
    
    Include the information of pseudo, duplicate, inaccessible file systems
    
- df -h(— human-readable)
    
    shows the sizes in powers of 1024 i.e in KB, MB, GB which are more human readable.
    
    ```bash
    user@user:~$ df -h /home/
    Filesystem      Size  Used Avail Use% Mounted on
    /dev/sda4        98G   24G   70G  26% /home
    ```
    
- df -T (—print-type)
    
    also print the type of file system
    
    ```bash
    user@user:~$ df -T
    Filesystem     Type     1K-blocks     Used Available Use% Mounted on
    udev           devtmpfs   3977808        0   3977808   0% /dev
    tmpfs          tmpfs       801396     2432    798964   1% /run
    /dev/sda7      ext4     154274224 20572580 125795292  15% /
    ```
    
- df -i (— inodes)
    
    Display the **inode** information instead of block usage.
    
    ```bash
    user@user:~$ df -i
    Filesystem        Inodes  IUsed     IFree IUse% Mounted on
    udev              994452    679    993773    1% /dev
    tmpfs            1001743   1521   1000222    1% /run
    /dev/sda7        9863168 329420   9533748    4% /
    ```
    
    **inode (**index node**):** Each inode stores the attributes and disk block locations of the object's data. 
    
- Filtering the output
    - (df -t <filesystem type>) Include certain filesystem type
        
        ```bash
        user@user:~$ df -t ext4
        Filesystem     1K-blocks     Used Available Use% Mounted on
        /dev/sda7      154274224 20582864 125785008  15% /
        /dev/sda4      102688032 24879344  72549424  26% /home
        ```
        
    - (df -x <type>) exclude certain filesysyem type
        
        ```bash
        user@user:~$ df -x ext4
        Filesystem     1K-blocks     Used Available Use% Mounted on
        udev             3977808        0   3977808   0% /dev
        tmpfs             801396     2432    798964   1% /run
        ```
        
- df —help
    
    To get information about the various options and their usage.