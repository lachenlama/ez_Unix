# Echo
<article>The echo command is a built-in Linux feature that prints out arguments as the standard output. echo is commonly used to display text strings or command results as messages.</article>
<br/>

### Echo Command Syntax

- The echo command in Linux is used to display a string provided by the user.


  > `echo [option] [string]`

- For example, use the following command to print **Hello, World!** as the output:

  > `echo Hello, World!`

<br/>

### Echo Command Options
- Use the `--help` argument to list all available echo command options:

  > `/bin/echo --help`

<br/>

### List of echo options
The echo command uses the following options:

>- -n: Displays the output while omitting the newline after it.
>- -E: The default option, disables the interpretation of escape characters.
>- -e: Enables the interpretation of the following escape characters:
>- \\: Displays a backslash character (\).
>- \a: Plays a sound alert when displaying the output.
>- \b: Creates a backspace character, equivalent to pressing Backspace.
>- \c: Omits any output following the escape character.
>- \e: The escape character, equivalent to pressing Esc.
>- \f: The form feed character, causes the printer to automatically advance to the start of the next page.
>- \n: Adds a new line to the output.
>- \r: Performs a carriage return.
>- \t: Creates horizontal tab spaces.
>- \v: Creates vertical tab spaces.
>- \NNN: Byte with the octal value of NNN.
>- \xHH: Byte with the hexadecimal value of HH.