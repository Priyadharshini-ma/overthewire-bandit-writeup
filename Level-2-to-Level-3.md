# Level 2 → Level 3

## Objective
Find the password for Bandit Level 3. The password is stored in a file with spaces in its name.

## Commands Used
ls -la  
cat -- "--spaces in this filename--"

## Explanation
- Listed all files with detailed information using `ls -la`.
- Identified a file named `--spaces in this filename--`.
- Used `cat --` to safely read a filename that begins with dashes.
- The file output contained the password for Level 3.
  
<img width="651" height="217" alt="image" src="https://github.com/user-attachments/assets/e42bf420-3ff7-42a7-b245-ced00aeebaac" />

## Password
MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx

## What I Learned
- How to handle filenames with spaces
- How to safely access files starting with special characters using `--`
