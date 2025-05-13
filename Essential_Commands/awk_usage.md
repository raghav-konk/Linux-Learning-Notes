# awk a.k.a Aho, Weinberger, and Kernighan (Name of the creators)
### Purpose
- Used for processing text data when dealing with files or streams of text
- Find lines that match with specific patterns
- Can also be used for printing, formatting and calculating values
## awk Syntax
```
awk options 'selection _criteria {action }' input-file > output-file
```
## Usage
### 1. Print only the first column in the standard output
```
awk '{ print $1 }' story.txt
```
This prints the only the first column of the output. Treats it as crude spreadsheet
### 2. Print lines with matching text
```
awk '/hello/ { print }' file.txt

```
This searches for hello in the given file and prints the lines that contains hello as output. 

### 3. Pairing with Delimiters
```
awk -F ',' '{ print $1 }' file.csv

```
Here comma is dreated as delimter, Need this in case out dataset use comma as delimiter instead of say spaces

### 4. Using Conditional Logic
```
awk '$3 > 50 { print $1, $3 }' data.txt

```
This uses conditional logic. Kinda like if. It prints first and third fields if the third field is greater than 50.