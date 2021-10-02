## ls
- "ls" is a command in the Linux/Unix system to list the computer files present in the folder you are working on at that particular time.
---

```bash
user@user:~$ ls
cd/  chmod/  CONTRIBUTING.md  df/  history/  LICENSE  ls/  README.md
```
- ls 
    Displays the files available in the current folder.

```bash
user@user:~$ ls -l
total 16
drwxr-xr-x 1 Owner staff    0 Oct  2 15:18 cd/
drwxr-xr-x 1 Owner staff    0 Oct  2 15:18 chmod/
-rw-r--r-- 1 Owner staff 4216 Sep 30 23:23 CONTRIBUTING.md
drwxr-xr-x 1 Owner staff    0 Oct  2 15:18 df/
drwxr-xr-x 1 Owner staff    0 Oct  2 15:18 history/
-rw-r--r-- 1 Owner staff 1094 Oct  1 11:41 LICENSE
drwxr-xr-x 1 Owner staff    0 Oct  2 14:42 ls/
-rw-r--r-- 1 Owner staff  954 Oct  2 15:18 README.md
```
- ls -l 
    1. Displays the permission given to the folder where:
        - d -> directory
        - r -> read
        - w -> write
        - x -> execute

    2. Displays the number of links to the content.

    3. Displays the name of the owner.

    4. Displays the group owner of content.

    5. Size of the file/folder in **bytes**.

    6. Modified data-time of the file/folder.

    7. File/Directory name.

```bash
user@user:~$ ls -lh
total 16K
drwxr-xr-x 1 Owner staff    0 Oct  2 15:18 cd/
drwxr-xr-x 1 Owner staff    0 Oct  2 15:18 chmod/
-rw-r--r-- 1 Owner staff 4.2K Sep 30 23:23 CONTRIBUTING.md
drwxr-xr-x 1 Owner staff    0 Oct  2 15:18 df/
drwxr-xr-x 1 Owner staff    0 Oct  2 15:18 history/
-rw-r--r-- 1 Owner staff 1.1K Oct  1 11:41 LICENSE
drwxr-xr-x 1 Owner staff    0 Oct  2 14:42 ls/
-rw-r--r-- 1 Owner staff  954 Oct  2 15:18 README.md
```
- ls -lh
    1. Dipslays the same as ls -l but provides the size in B,MB, GB,or TB when the file size is larger than 1024 bytes.

