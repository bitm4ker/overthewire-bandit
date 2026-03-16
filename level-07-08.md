# Level 7 → Level 8
## Objective
Find text within a file containing the flag.
## Key Concept
Filtering for text in a file with the "grep" command
## Commands Used
```bash
ls
grep "millionth" data.txt
```
## Why It Worked
This worked because in this case the command grep is used to find lines containing a specific text, as shown in the quotation marks in Commands Used.
## Note
Grep has several direct relevant usecases such as:
``` bash
# This filters by line
grep "text" filename
# This also filters by line but is case insensitive
grep -i "text" filename
# This searches across mutliple files or directories
grep -r "text" /path/to/dir
```
More usecases exist and will be noted in later labs.
## What I Learned
I learned to use the grep command to find text within a file, I also learned other usecases for grep.
## Summary
Using the grep command allows you to filter a file by line.
