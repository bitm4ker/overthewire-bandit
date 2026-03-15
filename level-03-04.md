Level 3 → Level 4

## Objective
Obtain the password which is stored in a hidden file within the *inhere* directory.

## Key Concept
Linux hidden files

## Commands Used
```bash
ls
cd inhere
find .
cat ./...Hiding-From-You
```

## Why It Worked
It worked because "find" is used to find files by name within a directory. In this example I inputted "find ." and it listed the hidden file.

## Note
In Linux, files and directories are hidden based on their name. Any file or folder beginning with a dot (.) in their name is hidden. EX:
``` bash
./...Hiding-From-You

```
This explains why I used "find ." with the dot specifically. 

Alternative:
Use "ls -a" this lists all files including ones beginning with a dot. (This is actually more common)
## What I Learned
I learned about hidden files and how they're handled on linux. I also learned how to find them with the "find" command to view and then the familar "cat" command to access hidden files.
## Summary
Overall, this level demonstrated the way to view hidden files and why they get hidden. 
