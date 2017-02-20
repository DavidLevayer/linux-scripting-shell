# Getting started

## Create your first script

* Open a terminal
* Create a new file (if needed):
```unix
touch my_script.sh
```
* Add permission to execute this file for all users:
```unix
chmod a+x my_script.sh
```
* Edit your file ; add fowllowing line:
```bash
#!/bin/bash
# My first bash script
echo 'hello world!'
```
* Execute your script:
```unix
./my_script.sh
```
* A welcome message should have been printed in your terminal

## Print in the terminal

```bash
echo hello world !
echo 'hello world!'
echo "hello world\!"
echo $var
# echo without new line
echo -n "do not print a new line"
```

```bash
# %s, %c, %d and %f are format substitution characters
# %-5s means left alignment (-) string (s) with specified width (5) 
printf "%-5s %-10s %-30s %-5s\n" Id Name Description Rating
printf "%-5s %-10s %-30s %-5.1f\n" 1 hello1 "hello1 description" 12.345
printf "%-5s %-10s %-30s %-5.1f\n" 2 hello2 "hello2 description" 9.8
```

```bash
# Text color codes:
#   0:   reset
#   30:  black
#   31:  red
#   32:  green
#   33:  yellow
#   34:  blue
#   35:  magenta
#   36:  cyan
#   37:  white

# Set color to red ; print 'Red text'; set color back to default
echo -e "\e[1;31mRed text\e[0m"

# Text background color codes:
#   0:   reset
#   40:  black
#   41:  red
#   42:  green
#   43:  yellow
#   44:  blue
#   45:  magenta
#   46:  cyan
#   47:  white

# Set color to red and background color to green ; print 'Hello text'; set color back to default
echo -e "\e[1;31;42mHello text\e[0m"
```

