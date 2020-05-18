# Terminal (Mac / Linux) Tips

### Get number of files in the directory

```
ls | wc -1
```

### List files by date modified (most recent first)

```
ls -ltrh
```

### Remove Mac's .DS_Store from a directory

```
find . -name ‘.DS_Store’ -type f -delete
```

### Ignore files that are greater than 50 MB (add to gitignore)

```
find . -size +50M | cat >> .gitignore
```

### Add a terminal shortcut (e.g., to ignore large files)

```
alias ignore-large-files="find . -size +50M | cat >> .gitignore"
```

