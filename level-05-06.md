# Level 5 → Level 6

## Objective
Access a file within the *inhere* directory with specific properties such as size and type.
## Key Concept
Hidden Files and File properties. 
## Commands Used
```bash
ls
find -size 1033c
cat "./.file2"
```

## Why It Worked
"find -size" searches for files matching a specific size, narrowing down results when multiple files exist
Example:
``` bash
# In this example it finds files with exactly 67 bytes in size
find -size 67c
```

## Note
The `find` command supports searching by file size using unit suffixes:
`c` = bytes, `k` = kilobytes, `M` = megabytes, `G` = gigabytes.
## What I Learned
I learned about the find command along with the unit suffixes which allow searching for a file using a specific size filter. 
## Summary
Overall, I used "find -size" along with the "c" suffix to find a specific file with a specific size.
