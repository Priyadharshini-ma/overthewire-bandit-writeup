# Level 13 → Level 14

## Objective
Find the password for Bandit Level 14. Login using an SSH private key instead of a password.

## Commands Used
scp -P 2220 bandit13@bandit.labs.overthewire.org:sshkey.private .  
chmod 600 sshkey.private  
ssh -i sshkey.private bandit14@bandit.labs.overthewire.org -p 2220  
cat /etc/bandit_pass/bandit14

## Explanation
- Copied the private SSH key from the Bandit server to the local machine using `scp`.
- Changed the permissions of the private key file to be readable only by the owner using `chmod 600`.
- Logged into the Bandit server as `bandit14` using the private key with the `ssh -i` option.
- Read the password for Bandit Level 14 from `/etc/bandit_pass/bandit14`.

<img width="1838" height="705" alt="image" src="https://github.com/user-attachments/assets/c3f8ec8d-1bd5-4963-b92b-3aa50fcd1038" />
<img width="762" height="700" alt="image" src="https://github.com/user-attachments/assets/7c21b726-b8cb-4206-a696-af446bde0671" />
<img width="770" height="405" alt="image" src="https://github.com/user-attachments/assets/11700dab-b7b7-4b49-97ed-2898b458b6cb" />


## Password
MU4WeTyJk8R0of1qqmcBPaLh7lDCPvS

## What I Learned
- How SSH key-based authentication works
- How to securely handle private keys
- How to use `scp` to copy files from a remote server
