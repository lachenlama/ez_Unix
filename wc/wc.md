## wc

"wc" stands for word count and does exactly that. Without any option you get the line-, word- and bytecount of the selected file.


```bash
user@user:~$ wc textfile.txt
144  319 4637 textfile.txt
```
The first Number represents the line-, second is the word- and last one the bytecount and if more than one file was selected, in the last row the total.

The folowing options are available:

- c return only the bytecount
    
```bash
user@user:~$ wc -c textfile.txt
4637 textfile.txt
```
- m return only the character count

```bash
user@user:~$ wc -c textfile.txt
4637 textfile.txt
```
- l return only the linecount

 ```bash
user@user:~$ wc -c textfile.txt
144 textfile.txt
```
- w return only the wordcount

```bash
user@user:~$ wc -c textfile.txt
319 textfile.txt
```
- L returns the length of the longest line

```bash
user@user:~$ wc -L textfile.txt
176 textfile.txt
```
