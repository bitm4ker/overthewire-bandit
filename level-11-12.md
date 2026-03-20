# Level 11 → Level 12

## Objective
Find the flag using Rot13.
## Key Concept
Rot13 in order to transform input text.
## Commands Used
```bash
ls
cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
```

## Why It Worked
Cat is to output the file/input so it can be processed by the next command tr. Tr (translate) is used to replace/transform characters within a file. In this level it performs character-by-character substituion based on the two sets given within the command. 'A-Za-z" is mapped to the corresponding character in "N-ZA-Mn-za-m" which implements the ROT13 cipher.
## Note
To explain using laymen explanation: "A-Za-z" matches all uppercase and lowercase letters, "N-ZA-Mn-za-m" shifts each letter 13 positions forward in the alphabet. (A to N, N to A)
EX:
``` bash
## Assuming xyz literally contains the letters xyz 
cat xyz | tr 'A-Za-z' 'N-ZA-Mn-za-m'
klm
```
Further notes for me:
For the first set A-Z matches all uppercase letters and a-z matches all lowercase letters, excluding no letters.
For the second set: N-Z matches the first 13 uppercase letters replacing A-M, A-M replaces N-Z, same for the lowercase letters.


## What I Learned
I learned Rot13 ciphering and in-depth review of it. I also learned that its self-reversing; applying it twice returns it into the original text.
## Summary
Rot13 translates text 13 characters ahead in the English Alphabet.
