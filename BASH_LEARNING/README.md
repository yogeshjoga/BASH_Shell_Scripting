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
        
        # echo with -x command this command will show you everything what you written in script and output as well as.
        # you should mention into shebang line as a -x, refer below command

        #!/bin/bash -x
        echo "Hello the world"
        echo "dear"
        echo ((2+3))
        # complete script will disply with output also
```
# Printing Strings That Contain Single Quotes 
```bash
        #!/bin/bash
        # if want to print the Quotes inside the code
        echo "hello dear i'm yogesh"
        # it will retrive the single quote inside the script  

```
# Printing Strings That Contain Double Quotes 
```bash
        #!/bin/bash
        # print the double quotes inside the code
        echo "my fav car is \"ROLL'S ROYCE\" "
        # it will return double quotes inside the ROLL'S ROYCE 


```
# Write to a File from Inside A Script 
```bash
        #!/bin/bash
        # create file and write the print statment insdie the file
        echo  " my name is yogesh joga, im a \"HACKER\" " > ./file.txt
        # it mean you pass the file name with extension 
        # ./ mean run command you can use( ./ or bash ) also
```
# Overwrite to a File from Inside A Script 
```bash
        #!/bin/bashb
        # create file and write the output as file write and override the file content
        echo "my name is balu, and im a Ethical Hacker" > ./file.txt
        # replace it
        echo "my name is yogesh, and im a Ethical Hacker" > ./file.txt

```
# Append to File Inside Script 
```bash
        #!/bin/bash
        # create file and write the output as file write and append the file content
        echo "my name is balu, and im a Ethical Hacker" > ./file.txt
        # append the 2nd line u cann add double angle brace
        echo "my name is yogesh, and im a Ethical Hacker" >> ./file.txt

```
# Single Line Comments 
```bash
        #!/bin/bash
        # if want to write the comment it won't be refelect to the code or script
        # so we can add the in front of the line of code "#"
        # hash is to be use as a single line comments
        echo "upper all lines are comments"

```
# Comments From Middle of Line 
```bash
        #!/bin/bash
         # middle of the line you can use hash only 
        echo "upper all lines are comments" # " hello "
        # im commenting the hello string in echo command line
```
# Multi Line Comments Using Heredocs 
```bash
        #!/bin/bash
        # now multi lines commenting
        <<THIS_IS_MULTI_LINE_COMMENTING
            INSIDE what you written this all things are 
            comments, it won't refelect the compile time
            on the code

        THIS_IS_MULTI_LINE_COMMENTING

```
# Simple Variable Usage 
```bash
        #!/bin/bash
        # bash support open data types it mean it won't except any data types
        # it will automatically converted strings and integers
        var="hello my name is yogi"
        # variable calling by using variable and dollar $
        echo $var
        # print the varable value 
```
# Multi Word Variables Combinations with Quotes 
```bash
        #!/bin/bash
        hello="this is the yogesh"
        dear="this is the linux"
        clas s="${hello} ${dear}"
        echo "${class}"
```
# HOME variable 
```bash
        # some of build in variables are there check into linux note
        #!/bin/bash
        var_path=$HOME
        echo "$var_path"
        ls "$var_path"
```
# USER variable 
```bash
        #!/bin/bash
        var_path=$USER
        echo "$var_path"
```
# HOSTNAME variable 
```bash
        #!/bin/bash
        var_path=$HOSTNAME
        echo "$var_path"
```
# Echo $HOME with Escape to Avoid Expansion 
```bash
        #!/bin/bash
        # we can use the \ forward slash 
        # to avoid the embedd links and quotes 
        echo "\$HOME"
        # run the script and see the output 
        # you can understand a lil
```
# Writing to file in HOME Directory Using HOME Environment Variable 
```bash
        #!/bin/bash
        cd $HOME
        echo "I like linux " > ./file.txt
        cat file.txt

```
# Simple Touch Command 
```bash
        #!/bin/bash
        touch file.txt
        ls
```
# Create a Symbol Link, Write To Linked File, Cat file 
```bash
        #!/bin/bash
        ln -s file.txt link1
        ls
        echo "now im writing inside the link1" >> link1
        cat link1 
```
# Chmod Command, Make Executable 
```bash
        #!/bin/bash
        chmod +x file.txt
```
# Chmod Command, Make Not-Writable, Try to Write to it 
```bash
        #!/bin/bash
        chmod -w  file.txt
         
```
# Chown File To Different User, Run ls before, after
```bash
        #!/bin/bash
        # bob is the user 
        # command "sudo adduser bob"
        chown bob file.txt
        sudo chown bob file.txt
```
# Underscore Variable, Touch File, Use Underscore Variable to Append to It 
```bash
        #!/bin/bash
        my_var="hello yogesh"
        touch file.txt
        echo "$my_var" >> file.txt
        cat file.txt
```
# Let Command Arithmetic 
```bash
        #!/bin/bash
        # init variables at a time 
        let a=4 b=5 c=a+b
        # calling variables
        echo "$a $b $c"

```
# 4 Basic Operators, Add, Subtract, Multiply, Divide 
```bash
        #!/bin/bash
        # init variables
        num1=10
        num2=20
        
        # add
        expr num1 + num2
        # sub
        expr num1 - num2
        # multi star will not allow in bash scripting lang so we need put \  slash infront of star
        expr num1 \* num2
        # div
        expr num1 / num2

```
# Increment a variable 3 times with Increment Operator 
```bash
        #!/bin/bash
        # increment the variable values 
        var=10
        echo $var
        # start increment
        var=$((var+=1))
        echo $var
        # 2nd time increment
        var=$((var+=1))
        echo $var
        # 3rd time increment
        var=$((var+=1))
        echo $var
        # printing every value after incrementing
```
# Decrement a variable 3 times with Decrement Operator 
```bash
        #!/bin/bash
         # decrement the variable values 
        var=10
        echo $var
        # start decrement
        var=$((var-=1))
        echo $var
        # 2nd time decrement
        var=$((var-=1))
        echo $var
        # 3rd time decrement
        var=$((var-=1))
        echo $var
        # printing every value after decrementing

```
# Echo Number Modulus Second Number 
```bash
        #!/bin/bash
        num1=10
        num2=4
        # it will give reminder value
        echo "$(($num1 % $num2))"

```
# Echo Number to Exponent of Second Number 
```bash
        #!/bin/bash
        num=$((8**2))
        echo "$num"

```
# Expr Command for Math 
```bash
        #!/bin/bash
        # exper function to make more math logics
        num1=20
        num2=10
        # operation
        # the expr command will perform action and print values also it is the advantage of this meth
        expr num1 + num2
        expr num1 - num2
        expr num1 \* num2
        expr num1 / num2
        expr num1 % num2
```
# Double Parenthesis for Math 
```bash
        #!/bin/bash
        num1=200
        num2=10
        # operation
        # this option will more complicated and we all are very lazy so we need shortcut only.....
        echo "$((num1 - $num2))" # inline printing the values
        echo "$((num1 + $num2))"
        echo "$((num1 \* $num2))"
        echo "$((num1 / $num2))"
        echo "$((num1 % $num2))"
```
# Double Parenthesis with Dollar Operator Assign to Variable
```bash
        #!/bin/bash
        num=100
        var=$((num+10))
        echo $var
```
# Multiplication has Precedence Over Addition Regardless of Order 
```bash
        #!/bin/bash
        var=$((3*(2+1)))
        echo "$var"

        new_var=$((2+3(*3)))
        echo $new_var

```
# Combine Two Strings In One Line With Variables 
```bash
        #!/bin/bash
        var1="HELLO THE WORLD"
        var2="this is bash"
        var3="hi this is yogesh joga"
        # two strings concatnation by using variables
        var4 ="${var1} ${var2} ${var3}"
        # concat new
        var1+="$var2"
        echo "$var1"
        echo "$var4"
```
# Combine Three Strings In One Line With Variables 
```bash
        #!/bin/bash

```
# Plus Equal Operator Combine Strings 
```bash
        #!/bin/bash

```
# Create Multi-Line String Variable with HEREDOC 
```bash
        #!/bin/bash

```
# Cat Multi-Line HEREDOC Text 
```bash
        #!/bin/bash

```
# If Conditional Statement 
```bash
        #!/bin/bash

```
# Logical And in Conditional Statement 
```bash
        #!/bin/bash

```
# Logical Or in Conditional Statement 
```bash
        #!/bin/bash

```
# If Elif Else Conditional Statement 
```bash
        #!/bin/bash

```
# Nesting If Conditions 
```bash
        #!/bin/bash

```
# Equal vs Double Equal Operator 
```bash
        #!/bin/bash

```
# Test Not Equal Strings 
```bash
        #!/bin/bash

```
# Test Two Strings Before or After alphabetically 
```bash
        #!/bin/bash

```
# Test String is Null 
```bash
        #!/bin/bash

```
# Test String is Not-Null
```bash
        #!/bin/bash

```
# Test Numerical Comparisons Greater then, Less then 
```bash
        #!/bin/bash

```
# Test Numerical Compare Greater Then Or Equal, Less Than Or Equal 
```bash
        #!/bin/bash

```
# Test Compare Numbers Are Equal 
```bash
        #!/bin/bash

```
# Test Compare Numbers Are Not-equal 
```bash
        #!/bin/bash

```
# Test File Exists 
```bash
        #!/bin/bash

```
# Test File Is Not Zero Size 
```bash
        #!/bin/bash

```
# Test File Is A Directory 
```bash
        #!/bin/bash

```
# File Is A Symbolic Link 
```bash
        #!/bin/bash

```
# Test File Has Read Permission 
```bash
        #!/bin/bash

```
# Test File Has Write Permission 
```bash
        #!/bin/bash

```
# Test File Has Execute Permission 
```bash
        #!/bin/bash

```