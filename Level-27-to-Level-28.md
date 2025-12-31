# Level 27 → Level 28

## Objective
Obtain the password for Bandit Level 28 by cloning a remote Git repository over SSH and reading its contents.

## Commands Used
cd /tmp  
git clone ssh://bandit27-git@bandit.labs.overthewire.org:2220/home/bandit27-git/repo  
cd repo  
cat README  

## Explanation
- Moved to the `/tmp` directory to work in a writable location.
- Cloned the remote Git repository using SSH.
- Entered the cloned repository.
- Read the `README` file, which contained the password for the next level.

<img width="733" height="511" alt="image" src="https://github.com/user-attachments/assets/afbfa86e-0321-40f6-a23d-7dc54864c319" />


## Password
Yz9IpL0sBcCeuG7m9uQFt8ZNpS4HZRcN

## What I Learned
- How to clone Git repositories over SSH
- How credentials can be exposed through repository files
- Why sensitive data should never be stored in plain text
