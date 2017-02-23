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

## useful variables
```bash
# Get current shell
echo $SHELL
```

## Useful commands
```bash
# Get environment variables available for specific process
# Replace '\0' with '\n' for better readability
cat /proc/$PID/environ | tr '\0' '\n'
```
