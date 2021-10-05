## Command name: rm 
Usage:
```
rm file_name
```

This command is used to delete a file from a directory. rm means to remove a file. <br>
It is recommended to use rm with -i. The -i ensures that there will be a confirmation before deleting the file.

### Other useful command options for removing a file(or multiple files):

- rm file1 file2: will remove both file1 and file2 in one command
- rm \*.txt: will remove all the text documents from the current directory
- rm -f file1: will remove file1 without any prompts for confirming even when the file is write protected
- rm -fv* file: will remove file from directory without a confirmation prompt in verbose mode

### Removing directories:

- rm -d dirname: will remove an empty directory named dirname
- rm -r dirname: will remove all the files from the dirname directory and also the directory itself
- rm -rf dirname: remocves all files inside the dirname directory and the directory without any confirmation prompts for write protected files of the directory
- rm -r dir1 dir2 dir3: will remove all the three directories completely
