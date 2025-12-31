# Level 30 → Level 31

## Objective
Find the password for Bandit Level 31 by inspecting Git tags in a repository.

## Commands Used
cd /tmp  
git clone ssh://bandit30-git@bandit.labs.overthewire.org:2220/home/bandit30-git/repo  
cd repo  
ls  
git tag  
git show secret  

## Explanation
- Cloned the Git repository for Bandit Level 30.
- Listed repository contents and found no visible password.
- Displayed available Git tags.
- Found a tag named `secret`.
- Used `git show secret` to reveal the password stored in the tag.

<img width="771" height="709" alt="image" src="https://github.com/user-attachments/assets/94b904fe-af44-48ec-b7ae-650ffcb8d07d" />


## Password
fb5S2xb7bRyFmAvQYQGEqsbhVyJqhnDy

## What I Learned
- Git tags can store sensitive information
- Secrets may exist outside branches and commit history
- Why repositories must be audited thoroughly before sharing
