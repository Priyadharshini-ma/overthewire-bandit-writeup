# Level 7 → Level 8

## Objective
Find the password for Bandit Level 8. The password is located in a file containing many entries.

## Commands Used
ls  
grep millionth data.txt  
grep millionth data.txt | awk '{print $2}'

## Explanation
- Listed files in the directory using `ls`.
- Identified the file `data.txt`.
- Used `grep millionth data.txt` to search for the line containing the word `millionth`.
- The matching line contained two fields.
- Used `awk '{print $2}'` to extract the second field, which is the password.

<img width="494" height="170" alt="image" src="https://github.com/user-attachments/assets/4b91a426-b1ed-4c3e-8fe2-aa4caf2d6736" />


## Password
dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc

## What I Learned
- How to search text files using `grep`
- How to extract specific fields from output using `awk`
- How to combine commands using pipes (`|`)
