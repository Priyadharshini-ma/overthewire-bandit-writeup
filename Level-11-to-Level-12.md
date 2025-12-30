# Level 11 → Level 12

## Objective
Find the password for Bandit Level 12. The password is encoded using ROT13.

## Commands Used
ls  
cat data.txt  
cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'

## Explanation
- Listed files in the directory using `ls`.
- Viewed the contents of `data.txt` using `cat`.
- Observed that the text was encoded using ROT13.
- Used the `tr` command to translate characters and decode the ROT13 text.
- The decoded output revealed the password for Level 12.

## Password
7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4

## What I Learned
- What ROT13 encoding is
- How to decode ROT13 using the `tr` command
- How character translation works in Linux
