# rm

`rm` is a unix command to remove files or directories present in the folder you are working on at that particular time.

```bash
rm [OPTION]... file...
```

---

## Description

**rm** removes the specified file. It can also be used to remove multiple files. But, it won't remove directories by default.

If the -I or --interactive=once option is given, and there are more than three files or 
the -r, -R, or --recursive are given, then rm prompts the user for whether to proceed with 
the entire operation. If the response is not affirmative, the entire command is aborted.

Otherwise, if a file is unwritable, standard input is a terminal, and the -f or --force 
option is not given, or the -i or --interactive=always option is given, rm prompts the 
user for whether to remove the file. If the response is not affirmative, the file is skipped.

|Tag| Description|
|---|---|
|-f, --force|ignore nonexistent files, never prompt.|
|-i|Prompt before every removal.|
|-I|Prompt once before removing more than three files, or when removing recursively. Less intrusive than -i, while still giving protection against most mistakes.|
|--interactive[=WHEN]|Prompt according to WHEN: never, once (-I), or always (-i). Without WHEN, prompt always.|
|--one-file-system|When removing a hierarchy recursively, skip any directory that is on a file system different from that of the corresponding command line argument.|
|--no-preserve-root|Do not treat '/' specially.|
|--preserve-root|Do not remove '/' (default).|
|-r, -R, --recursive|remove directories and their contents recursively.|
|-v, --verbose|explain what is being done.|
|--help|display this help and exit.|
|--version|output version information and exit.|

#### Examples

**Example 1**:

Remove file.txt

```bash
rm file.txt
```

**Example 2**:

Remove multiple files (file1.txt, file2.txt, file3.txt)

```bash
rm file1.txt file2.txt file3.txt
```

**Example 3**:

Remove all files in the working directory. If it is write-protected, you will be prompted before rm removes it

```bash
rm * 
```

**Example 4**:

Remove the directory dir1

```bash
rm -r dir1
```
