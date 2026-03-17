# Level 8 → Level 9

## Objective
Look for the flag by filtering file for a single nonduplicated (unique) string.
## Key Concept
Piping and filtering file via unique strings.

## Commands Used
```bash
ls
sort data.txt | uniq -u

```

## Why It Worked
The Sort command is used to sort lines of text files. Uniq is used to filter out adjacent duplicate lines from text. It reads the file and only outputs unique lines if duplicates are consecutive.
## Note
Uniq -u specifically only prints unique lines. 

## What I Learned
I learned about piping, (|) which is used in order to chain multiple commands as shown in the Commands Used part. I also learned about filtering for unique lines.
## Summary
Filter for unique lines using Uniq.
