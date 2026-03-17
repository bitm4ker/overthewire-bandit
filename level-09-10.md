# Level 9 → Level 10

## Objective
Filter files with string to extract human-readable strings (Lines).
## Key Concept
Extracting human-readable strings from a binary file via string.

## Commands Used
```bash
ls
strings data.txt | grep "=="
```

## Why It Worked
This worked because the Strings command extracted human-readable text from the file, while the grep command specifically filtered for "==" to find the strings beginning with various equal signs.
## Note
Piping shines in this example, allowing me to chain another command to reach my flag.
## What I Learned
I cemented piping and learned about the Strings command in conjunction with Grep to filter strings.
## Summary
Use Strings and Grep together to filter specific strings within a file.
