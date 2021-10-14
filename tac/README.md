# tac

`tac` read files and print them in reversed order, from last line to first line.

`tac [OPTION]... [FILE]...`.


Say you have a file named `file.txt` with the following content:

```
riley|19|student

martin|54|professor

kite|30|unknown

noomi|35|secretary
```

Using `tac`, you obtain this:
```
$ tac file.txt
noomi|35|secretary

kite|30|unknown

martin|54|professor

riley|19|student
```
Using `-s` you can pass a custom string as separator instead of newline. In combination with `-r`, the custom string will be interpreted as a regex.

```
$ tac -s "|" file.txt"
secretary
35|unknown

noomi|30|professor

kite|54|student

martin|19|riley|
```
