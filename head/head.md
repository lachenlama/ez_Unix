# Head

The head command is used to view the first lines of any text file. By default, it prints the first 10 lines of the specified files. If more than one file name is provided then data from each file is preceded by its file name. 

```bash
user@user:~$ head sample.txt
Muscowequan Muireadhach
Vilhelm Carolus
Tindra Aditi
Les Damián
Durk Kende
Sudhir Letîf
Fishel Yuina
Dipika Chava
Ismet Drusilla
Traci Simisola
```

## Options
1. -n <num>: Prints the first ‘num’ lines instead of first 10 lines. num is mandatory to be specified in command otherwise it displays an error. 


```bash
user@user:~$ head -n 5 sample.txt
Muscowequan Muireadhach
Vilhelm Carolus
Tindra Aditi
Les Damián
Durk Kende
```

2. -c <num>: Prints the first ‘num’ bytes from the file specified. Newline count as a single character, so if head prints out a newline, it will count it as a byte. num is mandatory to be specified in command otherwise displays an error. 


```bash
user@user:~$ head -c 11 sample.txt
Muscowequan%
```

3. -q: It is used if more than 1 file is given. Because of this command, data from each file is not precedes by its file name. 

Without using -q option

```bash
user@user:~$ head sample.txt sample2.txt
==> sample.txt <==
Muscowequan Muireadhach
Vilhelm Carolus
Tindra Aditi
Les Damián
Durk Kende
Sudhir Letîf
Fishel Yuina
Dipika Chava
Ismet Drusilla
Traci Simisola

==> sample2.txt <==
Afghanistan
Albania
Algeria
Andorra
Angola
Antigua and Barbuda
Argentina
Armenia
Australia
Austria
```

With using -q option

```bash
user@user:~$ head -q sample.txt sample2.txt
Muscowequan Muireadhach
Vilhelm Carolus
Tindra Aditi
Les Damián
Durk Kende
Sudhir Letîf
Fishel Yuina
Dipika Chava
Ismet Drusilla
Traci Simisola
Afghanistan
Albania
Algeria
Andorra
Angola
Antigua and Barbuda
Argentina
Armenia
Australia
Austria
```

4. -v: By using this option, data from the specified file is always preceded by its file name. 

```bash
user@user:~$ head -v sample.txt
==> sample.txt <==
Muscowequan Muireadhach
Vilhelm Carolus
Tindra Aditi
Les Damián
Durk Kende
Sudhir Letîf
Fishel Yuina
Dipika Chava
Ismet Drusilla
Traci Simisola
```
