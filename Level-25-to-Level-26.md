# Level 25 → Level 26

## Objective
Access Bandit Level 26 by using an SSH private key and escaping a restricted shell to obtain the password.

## Commands Used
ls  
file bandit26.sshkey  
exit  
scp -P 2220 bandit25@bandit.labs.overthewire.org:/home/bandit25/bandit26.sshkey .  
ssh -i bandit26.sshkey bandit26@bandit.labs.overthewire.org -p 2220  
:set shell=/bin/bash  
:shell  
cat /etc/bandit_pass/bandit26  

## Explanation
- Listed files and identified `bandit26.sshkey` as an SSH private key.
- Copied the SSH key to the local machine using `scp`.
- Logged into Bandit Level 26 using the private key.
- Encountered a restricted shell environment.
- Escaped the restricted shell by setting `/bin/bash` as the shell.
- Spawned a normal shell and read the password file.

<img width="511" height="139" alt="image" src="https://github.com/user-attachments/assets/1d2ac243-25cd-49d8-b8a2-386456ae7631" />

<img width="736" height="266" alt="image" src="https://github.com/user-attachments/assets/fc1f9a46-7954-42fe-8591-2f3fd8a963a2" />

<img width="239" height="71" alt="image" src="https://github.com/user-attachments/assets/64a50c89-f659-4e6e-a36a-aca69a2b5610" />

## Password
s0773xxkk0MXfdQfPRVr9L3jJBU0gCZ

## What I Learned
- How SSH key authentication works
- How restricted shells can be bypassed
- Why shell escape restrictions must be configured carefully
