# Level 6 → Level 7

## Objective
Find the password for Bandit Level 7. The password is stored somewhere on the server with specific ownership and size conditions.

## Commands Used
cd /  
find . -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null  
cat ./var/lib/dpkg/info/bandit7.password

## Explanation
- Changed to the root directory using `cd /`.
- Used the `find` command to search for files that:
  - Are regular files (`-type f`)
  - Are owned by user `bandit7`
  - Belong to group `bandit6`
  - Are exactly 33 bytes in size (`-size 33c`)
- Redirected permission errors to `/dev/null` using `2>/dev/null`.
- Located the file `bandit7.password`.
- Used `cat` to read the file and obtain the password.

## Password
morbNTDkSW6jILUOYmdoMaLNOIFVAaj

## What I Learned
- How to search the entire filesystem using `find`
- How to filter files by user, group, and size
- How to handle permission-denied errors using output redirection
