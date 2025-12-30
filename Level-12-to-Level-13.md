# Level 12 → Level 13

## Objective
Find the password for Bandit Level 13. The password is hidden inside a file that has been repeatedly compressed and encoded.

## Commands Used
mkdir /tmp/ctf  
cp data.txt /tmp/ctf  
cd /tmp/ctf  
file data.txt  
xxd -r data.txt > data  
file data  
mv data data.gz  
gzip -d data.gz  
file data  
mv data data.bz2  
bzip2 -d data.bz2  
file data  
mv data data.tar  
tar -xvf data.tar  
file data5.bin  
mv data5.bin a.tar  
tar -xvf a.tar  
file data6.bin  
mv data6.bin ak.bz2  
bzip2 -d ak.bz2  
file ak  
mv ak ak.tar  
tar -xvf ak.tar  
file data8.bin  
mv data8.bin ak.gz  
gzip -d ak.gz  
file ak  
cat ak

## Explanation
- Created a temporary working directory in `/tmp` to avoid modifying original files.
- Copied `data.txt` into the temporary directory.
- Used `file` to identify the file type at each stage.
- Converted hex dump back to binary using `xxd -r`.
- Repeatedly renamed and decompressed files using:
  - `gzip`
  - `bzip2`
  - `tar`
- Carefully followed each file transformation based on its detected type.
- After the final extraction, used `cat` to read the file containing the password.

<img width="791" height="529" alt="image" src="https://github.com/user-attachments/assets/feaca549-c4d8-408b-851f-3b8e26711308" />

<img width="542" height="180" alt="image" src="https://github.com/user-attachments/assets/1d80c316-199f-4472-bd64-9dd7cb0be3e9" />


## Password
F05dwFsc0cbaIiH0h8J2euks2vdTDwAn

## What I Learned
- How to analyze file types using the `file` command
- How to handle multiple layers of compression
- How to safely work in `/tmp`
- How CTF challenges chain multiple Linux concepts together
