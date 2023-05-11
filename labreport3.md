# Lab-Report-Week3-Researching Commands
I choose to focus on 'grep' commands and did some research on it. I get sources/help from web browsers and ChatGPT.

## Using '-r'(or '--recursive')
* Description: Recursively searches files and directories.
* Source: [GNU Grep Manual](https://www.gnu.org/software/grep/manual/grep.html#Recursive-Searching)

Example 1(Searching Files)
```
grep -r "error" ./technical/
```
This command searches for the term "error" in all files within the ./technical/ directory and its subdirectories.

Example 2(Searching Directories)
```
grep -r "pattern" ./technical/
```
This command searches for the pattern "pattern" in all files within the *./technical/* directory and its subdirectories.

## Using '-l' (or '--files-with-matches')
* Description: Only displays the names of files containing matches.
* Source: [GNU Grep Manual](https://www.gnu.org/software/grep/manual/grep.html#Recursive-Searching)

Example 1 (searching files):
```
grep -l "keyword" ./technical/*
```
This command searches for the keyword "keyword" in all files within the ./technical/ directory and displays only the names of files that contain a match.

Example 2 (searching directories):
```
grep -l "pattern" ./technical/*
```
This command searches for the pattern "pattern" in all files within the ./technical/ directory and displays only the names of files that contain a match.

## Using '-i' (or '--ignore-case')
* Description: Performs case-insensitive matching.
* Source: Source: [GNU Grep Manual](https://www.gnu.org/software/grep/manual/grep.html#Recursive-Searching)

Example 1 (searching files):
```
grep -i "word" ./technical/*
```
This command searches for the word "word" (ignoring case) in all files within the ./technical/ directory.

Example 2 (searching directories):
```
grep -i "pattern" ./technical/*
```
This command searches for the pattern "pattern" (ignoring case) in all files within the ./technical/ directory.

## Using '-v' (or '--invert-match')
* Description: Inverts the matching, displaying lines that do not match.
* Source: [GNU Grep Manual](https://www.gnu.org/software/grep/manual/grep.html#Recursive-Searching)

Example 1 (searching files):
```
grep -v "term" ./technical/*
```
This command searches for lines that do not contain the term "term" in all files within the ./technical/ directory.

Example 2 (searching directories):
```
grep -v "pattern" ./technical/*
```
This command searches for lines that do not match the pattern "pattern" in all files within the ./technical/ directory.

## Conclusions
By leveraging these command-line options, you can efficiently search for specific patterns, ignore case, and perform inverted matching with the grep command, making it a powerful tool for file and directory analysis.
