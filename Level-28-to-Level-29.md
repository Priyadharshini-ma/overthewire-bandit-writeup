# Level 28 → Level 29

## Objective
Find the password for Bandit Level 29 by inspecting the commit history of a Git repository.

## Commands Used
cd /tmp  
mkdir bob  
cd /tmp/bob  
git clone ssh://bandit28-git@bandit.labs.overthewire.org:2220/home/bandit28-git/repo  
cd repo  
ls  
cat README.md  
git log -p  

## Explanation
- Created a working directory in `/tmp`.
- Cloned the Bandit Level 28 Git repository.
- Read the `README.md` file, which did not contain the password.
- Used `git log -p` to inspect previous commits.
- Found the password exposed in an earlier commit.

<img width="897" height="661" alt="image" src="https://github.com/user-attachments/assets/de554782-1c80-4ce0-a0ca-ee76eaaf8d65" />

<img width="343" height="332" alt="image" src="https://github.com/user-attachments/assets/b46bb46a-ecef-499d-a86e-7d4898463ece" />

<img width="826" height="658" alt="image" src="https://github.com/user-attachments/assets/0c442496-832d-422f-b9b8-630eb75b2777" />

<img width="443" height="195" alt="image" src="https://github.com/user-attachments/assets/953aa690-7865-4ebd-bba0-79e8892a2279" />


## Password
4pT1t5DENaYuqnqvadYs1oE4QLCdjmJ7

## What I Learned
- How Git commit history preserves deleted data
- Why secrets should never be committed to version control
- How `git log -p` helps analyze changes over time
