# cut

`cut` is a command to manipulate files and print desired parts of their content.

Say you have this csv file `bank.csv`:
```
NAME,IBAN,PIN
Keane,AD0853632164414039197146,1141
Fitzgerald,BA679412748100653125,8237
Lewis,RS66949383118416984785,6498
Mason,KZ356778987468572471,9652
Porter,TN5774446762791782622435,2783
```

- You can use `cut` to print the first byte of each row with the `-b` option:
```
$ cut -b 1 bank.csv
N
K
F
L
M
P
```
- You can do the same thing as above with `-c` to select characters.
```
$ cut -c 1 bank.csv
N
K
F
L
M
P
```
Or you can pass a range to select from the second character to the tenth:
```
$ cut -c 2-10 bank.csv
AME,IBAN,
eane,AD08
itzgerald
ewis,RS66
ason,KZ35
orter,TN5
```

- You can also select fields from your files using `-f` option.\
By default, `cut` will use tabulation as delimiter, but you can pass another one with the `-d` option. Let's select the first and third fields of our csv file, using comma as delimiter:
```
$ cut -d, -f 1,3
NAME,PIN
Keane,1141
Fitzgerald,8237
Lewis,6498
Mason,9652
Porter,2783
```

Note that `-b`, `-c` and `-f` are mutually exclusize. You cannot use both at the same time.