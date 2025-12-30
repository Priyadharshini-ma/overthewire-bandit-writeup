# Level 19 → Level 20

## Objective
Find the password for Bandit Level 20 by executing a program that runs commands with higher privileges.

## Commands Used
ls  
./bandit20-do  
./bandit20-do cat /etc/bandit_pass/bandit20

## Explanation
- Listed the files in the directory using `ls`.
- Found an executable file named `bandit20-do`.
- The program allows executing commands as the user `bandit20`.
- Used `./bandit20-do cat /etc/bandit_pass/bandit20` to read the password file.
- The output revealed the password for Level 20.

<img width="717" height="165" alt="image" src="https://github.com/user-attachments/assets/a1b720a6-3b68-47ed-8e8b-38814d6d73a4" />


## Password
0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO

## What I Learned
- How setuid programs work
- How commands can be executed with another user’s privileges
- Why privilege escalation must be handled carefully
