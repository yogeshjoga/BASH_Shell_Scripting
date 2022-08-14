# BASH PART ONE : 1 BASICS AND LITTLE SCRIPTS
```bash

```
# Basic fundamentals of BASH_SCRIPTING
```bash
        Bash is the linux scripting lang...
        # know abt th "SHEBANG"
        # What is "shebang"?
        # well! shebang will provide to connect the system.
        # if you use any computer with operating system you can indirectly interact with the shell.
        # if you use a terminal every time on any linux OS. It's connect to the shell only
        <<ABT_SHEBANG 
        We can mention it on Top of the script as like "#!/bin/bash or #!/bin/sh 
        both are same, usage but lil different...

        This script instructs the INTERNAL CALLS THE SHELL to start an interperting
        the code/script line by line manner.

        some examples in shebang command lines using in scripting langs
        There are: 
                    #!/bin/sh: It is used to execute the file using sh, which is a Bourne shell, or a compatible shell
                    #!/bin/csh: It is used to execute the file using csh, the C shell, or a compatible shell.
                    #!/usr/bin/perl -T: It is used to execute using Perl with the option for taint checks.
                    #!/usr/bin/php: It is used to execute the file using the PHP command-line interpreter.
                    #!/usr/bin/python -O: It is used to execute using Python with optimizations to code.
                    #!/usr/bin/ruby: It is used to execute using Ruby.

        ABT_SHEBANG




```
# Simple Hello World Script 

```bash
        #!/bin/bash
        echo "Hello the World!"
```
# Echo Command Without Newlines 
```bash
        #!/bin/bash
        # please vist comment section, single line and multi line

        # echo with -n flag 
        echo -n "Hello the "
        echo "world"
        # these two lines print in as like Hello the world it won't create a new line
        # minus n mean remove new line that's it
```
# String Concatenation With Echo 
```bash 
        #!/bin/bash
        # concat mean adding two string values
        # how we can add two strings?
        # just see below script
        echo "Hello "   "the "   "world!"
        # above line will print in single line only it won't be create a new line 
        # that's it bash is very easy lang, you can grab easily.....
```
# String Continuation Character 
```bash
        #!/bin/bash
        # bash_scripting 
        # you can write a echo command in single line, And continuation in new lines
        # you can use echo with back slash '\'
        echo "hello" "the " \  
                        "world" 
        # In echo command line we can give the back slash it will create continuation on 
        # next line on going 

```
# Echo with Tab Characters
```bash
        #!/bin/bash
        # escape char's in bash, we can use echo with -e flag 
        echo -e "\t Hello the world"
        # back slash t  --\t  this token provide TAB Space
```
# Echo with Newline Characters 
```bash
        #!/bin/bash
        # echo with new line token as similar into TAB Space
        echo -e "\n Hello the world"   "\n this is \n yogesh"
        # just run the command you can know abt it, Flow of the code

```
# Echo with -x to Display All Commands 
```bash

```
# Printing Strings That Contain Single Quotes 
```bash

```
# Printing Strings That Contain Double Quotes 
```bash

```
# Write to a File from Inside A Script 
```bash

```
# Overwrite to a File from Inside A Script 
```bash

```
# Append to File Inside Script 
```bash

```
# Single Line Comments 
```bash

```
# Comments From Middle of Line 
```bash

```
# Multi Line Comments Using Heredocs 
```bash

```
# Simple Variable Usage 
```bash

```
# Multi Word Variables Combinations with Quotes 
```bash

```
# HOME variable 
```bash

```
# USER variable 
```bash

```
# HOSTNAME variable 
```bash

```
# Echo $HOME with Escape to Avoid Expansion 
```bash

```
# Writing to file in HOME Directory Using HOME Environment Variable 
```bash

```
# Simple Touch Command 
```bash

```
# Create a Symbol Link, Write To Linked File, Cat file 
```bash

```
# Chmod Command, Make Executable 
```bash

```
# Chmod Command, Make Not-Writable, Try to Write to it 
```bash

```
# Chown File To Different User, Run ls before, after
```bash

```
# Underscore Variable, Touch File, Use Underscore Variable to Append to It 
```bash

```
# Let Command Arithmetic 
```bash

```
# 4 Basic Operators, Add, Subtract, Multiply, Divide 
```bash

```
# Increment a variable 3 times with Increment Operator 
```bash

```
# Decrement a variable 3 times with Decrement Operator 
```bash

```
# Echo Number Modulus Second Number 
```bash

```
# Echo Number to Exponent of Second Number 
```bash

```
# Expr Command for Math 
```bash

```
# Double Parenthesis for Math 
```bash

```
# Double Parenthesis with Dollar Operator Assign to Variable
```bash

```
# Multiplication has Precedence Over Addition Regardless of Order 
```bash

```
# Combine Two Strings In One Line With Variables 
```bash

```
# Combine Three Strings In One Line With Variables 
```bash

```
# Plus Equal Operator Combine Strings 
```bash

```
# Create Multi-Line String Variable with HEREDOC 
```bash

```
# Cat Multi-Line HEREDOC Text 
```bash

```
# If Conditional Statement 
```bash

```
# Logical And in Conditional Statement 
```bash

```
# Logical Or in Conditional Statement 
```bash

```
# If Elif Else Conditional Statement 
```bash

```
# Nesting If Conditions 
```bash

```
# Equal vs Double Equal Operator 
```bash

```
# Test Not Equal Strings 
```bash

```
# Test Two Strings Before or After alphabetically 
```bash

```
# Test String is Null 
```bash

```
# Test String is Not-Null
```bash

```
# Test Numerical Comparisons Greater then, Less then 
```bash

```
# Test Numerical Compare Greater Then Or Equal, Less Than Or Equal 
```bash

```
# Test Compare Numbers Are Equal 
```bash

```
# Test Compare Numbers Are Not-equal 
```bash

```
# Test File Exists 
```bash

```
# Test File Is Not Zero Size 
```bash

```
# Test File Is A Directory 
```bash

```
# File Is A Symbolic Link 
```bash

```
# Test File Has Read Permission 
```bash

```
# Test File Has Write Permission 
```bash

```
# Test File Has Execute Permission 
```bash

```