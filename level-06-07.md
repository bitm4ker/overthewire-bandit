# Level 6 → Level 7

## Objective
Find the password stored somewhere on the server with specific user, group, and size properties. 
## Key Concept
Server wide search with find filters
## Commands Used
```bash
## Searches for a file in root with those specific properties 
find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
## Simply prints the file we were looking for
cat /var/lib/dpkg/info/bandit7.password
```

## Why It Worked
The find command with / searches in root, not just the home directory I was currently in. Using -user, -size, and -group allows me to filter precisely in order to easily find that specific file.
2>/dev/null Also suppresses any "permission denied" responses.

## What I Learned
I learned how to find a file within root, and how to filter more precisely.

## Summary
Filter files more precisely using the find command, and searching within root.
