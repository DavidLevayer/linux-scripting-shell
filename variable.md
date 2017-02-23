# Variables

## Basics

```bash
# Assign a variable
var=value
var='value with spaces'

# Print a variable
echo $var
echo ${var} # same as $var
echo ${var}foo # curly brackets allow to concat without ambiguity
echo "$var" # print $var as a single word, even if it contains white spaces

# String length
length=${#var}
```

## Environment variables

These variables are not defined in the current process/script, but are received from the parent processes. They can be accessed the same way classic variables are accessed.

* useful variables
```bash
# Get current shell
echo $SHELL
```

* Useful commands
```bash
# Get environment variables available for specific process
# Replace '\0' with '\n' for better readability
cat /proc/$PID/environ | tr '\0' '\n'
```

## Math calculations

```bash
a=4
b=5

res=$a+$b # res equals '4+5'
let res=$a+$b # res equals '9'
let res=a+b # res equals '9'
let res=$[ a + b ] # res equals to '9'
let res=$(( a + b )) # res equals to '9'

let a++ # a equals '5'
let b+=5 # b equals '10'

x=4
echo "4*3" | bc # print '12'
echo "4*3.14" | bc # print '12.56'
echo "scale=1; 3/8" | bc # print '0.3'
echo "obase=2;$x" | bc # Switch to base 2; print '100'
echo "sqrt($x)" | bc # print '2'
echo "$x^2" | bc # print '16'
```
