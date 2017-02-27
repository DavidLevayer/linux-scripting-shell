# Code snipplets

This section expose a list of useful code snipplets.

* [Check for super user](snipplet.md#check-for-super-user)
* [Ask for password](snipplet.md#ask-for-password)

## Check for super user

```bash
if [ $UID -ne 0 ]; then
  echo "Non root user. Please run as root."
else
  echo "Root user"
fi
```

## Ask for password

```bash
echo -e "Enter password: "
stty -echo # Disable console output
read password
stty echo # Enable console output
echo Password read: $password
```
