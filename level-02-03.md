# Level 2 → Level 3
## Objective
Access the password stored in filename "--spaces in this filename--" located in the home directory.
## Key Concept 
Shell whitespace parsing
## Commands Used
```bash
ls
cat ./"--spaces in this filename--"
```
## Why It Worked
The shell interprets spaces in filenames as separate arguments because whitespace (spaces, tabs, and newlines) is the default delimiter (a character or sequence of characters used to separate a string or line of text) used to split command lines into individual arguments. ("Arguments" in bash are values you type after a script name or command.)
EX:
```bash
# Shell sees this as two arguments: "ARGUMENT" and "ONE"
cat ARGUMENT ONE
# Shell sees this as one argument: "ARGUMENT ONE"
cat "ARGUMENT ONE"
```
## Note
Because of the way whitespace is interpreted, Linux users prefer filenames without spaces.
## What I Learned
Overall, I learned what the shell interprets whitespace as. I also learned how to open filenames with spaces by specifying the path using "./" and wrapping the filename in quotation marks. (example in "Commands Used")
