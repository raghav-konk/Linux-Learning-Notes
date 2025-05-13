# Find and Xargs in Linux

### Purpose of find
- Find files based on type, size etc. in a file system
- Find files based on specific permission set



### Purpose of xargs
- It takes input and turns it into arguments for another command.
- Workaround when command piping does not work.

## find Syntax
```
find . -name "file.txt"
```
searches for file.txt in the entire file system


## Find Usage
### 1. Use -iname for case-insensitivity
```
find . -iname "file.txt"

```

### 2. Find files by extension
```
find . -name "*.mp4"
``` 

### 3. Find directories
```
find . -type d -name "backup"
```
### 4. Find files modified in the last 7 days
```
find . -mtime -7

```
### 5. Find files larger than 100MB
```
find . -type f -size +100M

```
### 6. Find and delete
```
find . -name "*.tmp" -delete
```