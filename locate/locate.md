## locate
- "locate" is a command to locate a file.
---
```bash
user@user:~$ locate searchword
    Lists all files containing the searched word, include there location.
```
```bash
user@user:~$ locate -i -l 2 searchword
user@user:~$ /home/user/images/searchword_image.png
user@user:~$ /home/user/documents/searchword.txt

    -i Makes the search case-insensitive.
    -l Limits the output to the given number
```

```bash
user@user:~$ locate -c searchword
2
    -c Returns only the count of files found
```
