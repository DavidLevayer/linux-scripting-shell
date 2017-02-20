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
```

```bash
printf "%-5s %-10s %-30s %-5s\n" Id Name Description Rating
printf "%-5s %-10s %-30s %-5.1f\n" 1 hello1 "hello1 description" 12.345
printf "%-5s %-10s %-30s %-5.1f\n" 2 hello2 "hello2 description" 9.8
```

