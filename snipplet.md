# Code snipplets

This section expose a list of useful code snipplets.

* [Check for super user](snipplet.md#check-for-super-user)

## Check for super user

```bash
if [ $UID -ne 0 ]; then
  echo "Non root user. Please run as root."
else
  echo "Root user"
fi
```
