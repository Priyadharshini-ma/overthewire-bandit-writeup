# Level 16 → Level 17

## Objective
Find the password for Bandit Level 17 by connecting to an SSL-enabled service that provides an SSH private key.

## Commands Used
ncat --ssl localhost 31790  
chmod 600 key17  
ssh -i key17 bandit17@bandit.labs.overthewire.org -p 2220  
cat /etc/bandit_pass/bandit17

## Explanation
- Connected to an SSL-enabled service on port `31790` using `ncat --ssl`.
- Submitted the password for Bandit Level 16 to the service.
- Received a private SSH key (`key17`) from the service.
- Changed the permissions of the private key to be owner-readable only using `chmod 600`.
- Logged in as `bandit17` using SSH key-based authentication.
- Read the password for Bandit Level 17 from `/etc/bandit_pass/bandit17`.

<img width="653" height="602" alt="image" src="https://github.com/user-attachments/assets/8675c09f-437f-48da-b0c6-319d9edcf7ba" />
<img width="652" height="573" alt="image" src="https://github.com/user-attachments/assets/4521544f-7b06-4e8f-811e-1da0d6bf4729" />
<img width="650" height="62" alt="image" src="https://github.com/user-attachments/assets/c5b22cb1-b5af-45e3-8e98-b04467aab2f2" />


## Password
EREvavePLFHtFlEsjn3hyzmlvSuSAcRD

## What I Learned
- How SSL services can return sensitive data securely
- How to use SSH private keys obtained dynamically
- Importance of correct file permissions for SSH keys
