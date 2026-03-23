# Level 12 → Level 13

## Objective
Perform a reverse Hexdump within layers

## Key Concept
Reversing Hexdumps 
## Commands Used
```bash
## Methods vary but this is how I personally solved it
## Extracting is repeated mutliple times in this walkthrough 
## I do this often to make sure I work with the correct files
ls
## Creates a unique temporary directory with a hard to guess name
mktemp -d
## Enters said directory 
cd /tmp/tmp.hardtoguess
## copies data.txt into the directory 
cp ~/data.txt //tmp/tmp.hardtoguess/
ls
## Prints data.txt
cat data.txt
## Reverses the hexadecimal dump data.txt back into binary form 
xxd -r data.txt output.txt
ls
cat output.txt
## Checks file type 
file output.txt
## Renames the file to output.gz to tell Linux to treat it as a gzip file, content is unchanged
mv output.txt output.gz
## Used to decompress the file, removes .gz and restores the file into its original state with attributes such as name, timestamp, ownership, and mode 
gunzip output.gz
ls
file output
## Decompresses the file compressed with bzip2
bunzip2 output
ls
file output.out
mv output.out output.gz
gunzip output.gz
ls
file output
## In this usecase tar is used to extract the file, x which stands for extract tells tar to extract files from an archive (file that bundles multiple files and folders) f just specifies the file which is why output follows it right after 
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
