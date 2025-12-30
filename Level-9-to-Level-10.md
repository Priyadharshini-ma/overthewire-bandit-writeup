# Level 9 → Level 10

## Objective
Find the password for Bandit Level 10. The password is hidden inside a file that contains non-printable characters.

## Commands Used
ls  
strings data.txt | grep "="

## Explanation
- Listed files in the directory using `ls`.
- Identified the file `data.txt`.
- Used `strings` to extract human-readable strings from the file.
- Piped the output to `grep "="` to filter lines containing an equals sign.
- The matching line revealed the password for Level 10.

<img width="415" height="339" alt="image" src="https://github.com/user-attachments/assets/26269e82-ba12-4979-a13a-8b626f3126c7" />


## Password
FGUW5ilLVJrxX9kMYMmN4MgbpfMiqey

## What I Learned
- How to extract readable text from binary files using `strings`
- How to filter specific patterns using `grep`
- How to combine commands using pipes (`|`)
