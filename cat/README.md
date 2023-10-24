# cat (concatenate)

-cat is a frequently used command in Linux/Unix-like operating systems.  
-cat allows us to create single or multiple files, view content of a file, concatenate files and redirect output in terminal or files.

### Usage: 
```cat [OPTION] [FILE]```

## Diplay contents of a file
```
[nga1hte@ubuntu ~]# cat /etc/passwd 
root:x:0:0:root:/root:/bin/bash
bin:x:1:1:bin:/bin:/sbin/nologin
nga1hte:x:500:500::/home/nga1hte:/bin/bash
```

## Diplay multiple file contents
```
[nga1hte@ubuntu ~]# cat hello.txt helloworld.txt 
hello
helloworld
```

## Display line numbers
```
[nga1hte@ubuntu ~]# cat -n text.txt 
1 Text is
2 just a 
3 random file
```
Read more about [cat](https://man7.org/linux/man-pages/man1/cat.1.html) 

