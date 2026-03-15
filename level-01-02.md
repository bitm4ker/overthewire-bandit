# Level 1 → Level 2

## Objective
Access file "-" in the home directory in order to obtain the password.
## Commands Used
```bash
ls
cat ./-
```

## Why It Worked

'cat ./-" works because dashes behave in a peculiar way in bash. "-" is used as a filename placeholder, it represents standard input or standard output. "./" was needed to specify the exact path to the filename "-".
## What I Learned
I learned that "-" is seen in a unique way in bash. I also learned how to open a file with the name "-' via specifying the path. EX:
``` bash
cat ./-filename
```
