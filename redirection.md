# Pipe, descriptors and redirection

```bash
# 0 - stdin
# 1 - stdout
# 2 - stderr

# Redirect to file; if file exists, it is replaced
echo "hello world!" > file.txt
# Redirect to file; add string at the end of the file
echo "hello world!" >> file.txt
# Redirect outputs into stdout.txt and errors into stderr.txt
cmd 1>stdout.txt 2>stderr.txt
# Redirect both outputs and errors into print.txt
cmd 2>&1 print.txt
cmd &> print.txt
# Redirect all outputs to nothing/null (nothing will be printed)
cmd &> /dev/null

# Read data from file and use them as command args
cmd < file.txt

# Print in console AND redirect to file
# Note: tee -a appends to file instead of overwrite
echo hello world | tee out.txt
```

