# grep

Grep stands for "Global regular expression print".
It is used to search a **regular expression** (pattern of characters) in a file.

#### Creating sample file
```bash
user@user:~$ cat > sample
I eat Apple and Banana
Horse is a domestic animal
Monkey eats Banana
dog barks
kite flies
```

#### Finding word "Apple" and "dog" in sample
```bash
user@user:~$ cat sample | grep Apple
I eat Apple
user@user:~$ cat sample | grep dog
dog barks
user@user:~$ cat sample | grep "o"
Horse is a domestic animal
Monkey eats Banana
dog barks
```

## Options 
| Option     | Use |
| ----------- | ----------- |
| -i | For case insensitive search|
| -v  | Select non-matching lines|
| -w | Search only whole word |
| -c | Print count of matching lines |
| -n | Prefix lines in output with line numbers |

#### grep -i tosearch 
```bash
user@user:~$ cat sample | grep -i DOG
dog barks
```

#### grep -v tosearch 
```bash
user@user:~$ cat sample | grep -v domestic
I eat Apple
Monkey eats Banana
dog barks
kite flies
```
#### grep -n tosearch 
```bash
user@user:~$ cat sample | grep -ni banana
1:I eat Apple and Banana
2:Monkey eats Banana
```
#### grep -c tosearch 
```bash
user@user:~$ cat sample | grep -ci banana
2
```