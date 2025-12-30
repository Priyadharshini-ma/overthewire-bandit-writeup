# Level 5 → Level 6

## Objective
Find the password for Bandit Level 6. The password is stored in a file that matches specific properties.

## Commands Used
ls  
cd inhere  
find . -type f -size 1033c -readable ! -executable  
cat ./maybehere07/.file2

## Explanation
- Listed files using `ls`.
- Entered the directory `inhere`.
- Used the `find` command to search for files that are:
  - Regular files (`-type f`)
  - Exactly 1033 bytes in size (`-size 1033c`)
  - Readable (`-readable`)
  - Not executable (`! -executable`)
- Located the file `./maybehere07/.file2`.
- Used `cat` to read the file and obtain the password.

## Password
HWasnPhtq9AVKe0dmk45nxy20cvUa6EG

## What I Learned
- How to use the `find` command with multiple conditions
- How to filter files based on size, permissions, and type
