# grep a.k.a Global Regular Expression Print (GREP)
### Purpose
- Searching text
- Manipulating Text Patterns
- Finding text patterns within Files

## GREP Syntax
```
grep [option] pattern_string [file_name]
```
## Usage
### 1. Ignoring Case Sensitivity
```
grep -i hello story.txt
```
This searches for the hello in a file called story.txt. Ignores the case sensitivity.

### 2. Recursive Pattern search
```
grep -iR hello dir_name
```
This searches for hello in the given directory recursively. Since we paired it with i option, this should be case insensitive. It gives out the files names where "hello' was seen in the given directory.