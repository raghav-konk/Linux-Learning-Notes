# sed a.k.a Stream Editor
### Purpose
- Basically acts like a find and replace tool in any Word editor programs like MS word etc.
- Used for Text manipulation and stream editing. 
- Perform batch operations on text editing
## sed Syntax
```
sed [options] 'command' [inputfile...]
```
## Usage
### 1. Replace first occurrence of "apple" with "orange":
```
sed 's/apple/orange/' fruits.txt
```

### 2. Replace all occurrences
```
sed 's/apple/orange/g'
``` 
g indicates global here.

### 3. Replace only on specific line (e.g., line 3)
```
sed '3s/apple/orange/' fruits.txt

```
### 4. Delete empty lines:
```
sed '/^$/d' file.txt
```
### 5. Delete specific lines: (Line 5 here)
```
sed '5d' file.txt
```
