# Level 18 → Level 19

## Objective
Find the password for Bandit Level 19 when the shell immediately logs you out after login.

## Commands Used
ssh bandit18@bandit.labs.overthewire.org -p 2220 cat readme

## Explanation
- Normally, logging in as `bandit18` immediately logs the user out.
- Used SSH to directly execute a command (`cat readme`) during login.
- This allowed reading the `readme` file without entering an interactive shell.
- The file contained the password for Bandit Level 19.

<img width="670" height="321" alt="image" src="https://github.com/user-attachments/assets/35fafeea-b469-4d09-be46-fe94f4f247cc" />

## Password
cGWpMaKXVwDUNgPAVJbWYuGHVn9zl3j8

## What I Learned
- How to execute commands directly over SSH
- How to bypass restricted interactive shells
- How SSH can be used non-interactively
