# Level 12 → Level 13

## Objective
Perform a reverse Hexdump within layers

## Key Concept
Reversing Hexdumps 
## Commands Used
```bash
## Methods vary but this is how I persoanlly solved it
ls
mktemp -d
cd /tmp/tmp.hardtoguess
cp ~/data.txt //tmp/tmp.hardtoguess/
ls
cat data.txt
xxd -r data.txt output.txt
ls
cat output.txt
file output.txt
mv output.txt output.gz
gunzip output.gz
ls
file output
bunzip2 output
ls
file output.out
mv output.out output.gz
gunzip output.gz
ls
file output
tar xf output
ls
file data5.bin
tar xf data5.bin
ls
file data6.bin
bunzip2 data6.bin
file data6.bin
bunzip2 data6.bin
file data6.bin.out
tar xf data6.bin.out
ls
file data8.bin
mv data8.bin data8.gz
gunzip data8.gz
file data8
cat data8
FLAG
```

## Why It Worked
*2-3 sentences max.*

## Note
*Optional.*

## What I Learned
*One or two sentences.*

## Summary
*One sentence.*
