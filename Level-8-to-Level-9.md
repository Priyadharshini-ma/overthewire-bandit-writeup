# Level 8 → Level 9

## Objective
Find the password for Bandit Level 9. The password is the only line of text that occurs once in the file.

## Commands Used
ls  
sort data.txt | uniq -u

## Explanation
- Listed files in the directory using `ls`.
- Identified the file `data.txt`.
- Used `sort` to sort all lines in the file.
- Used `uniq -u` to display the line that appears only once.
- The unique line contained the password for Level 9.

## Password
4CKMh1JI91bUIZZPXDQGanaL4xvAg0JM

## What I Learned
- How `sort` works with text files
- How to find unique lines using `uniq -u`
- How to combine commands using pipes (`|`)
