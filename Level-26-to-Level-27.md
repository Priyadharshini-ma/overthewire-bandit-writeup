# Level 26 → Level 27

## Objective
Obtain the password for Bandit Level 27 by leveraging a SUID binary to execute commands with higher privileges.

## Commands Used
ssh -i bandit26.sshkey bandit26@bandit.labs.overthewire.org -p 2220  
:set shell=/bin/bash  
:shell  
ls  
./bandit27-do  
./bandit27-do cat /etc/bandit_pass/bandit27  

## Explanation
- Logged into Bandit Level 26 using the provided SSH private key.
- Escaped the restricted shell to obtain a normal bash shell.
- Listed files and discovered a SUID binary named `bandit27-do`.
- Used the SUID binary to execute a command as Bandit Level 27.
- Read the password file for the next level.

<img width="413" height="82" alt="image" src="https://github.com/user-attachments/assets/8203e615-f887-4acc-b481-b84fe3432315" />

<img width="558" height="211" alt="image" src="https://github.com/user-attachments/assets/92d28ea0-d08a-4a58-b9df-6fc256222bbc" />


## Password
upsNCc7vzaRDx6oZC6GiR6ERwe1MowGB

## What I Learned
- How SUID binaries can be abused to escalate privileges
- Why executing arbitrary commands via SUID programs is dangerous
- The importance of proper permission management
