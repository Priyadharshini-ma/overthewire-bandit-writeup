# Level 29 → Level 30

## Objective
Retrieve the password for Bandit Level 30 by exploring different branches in a Git repository.

## Commands Used
cd /tmp/repo  
cat README.md  
git branch  
git branch -a  
git checkout dev  
git log -p  

## Explanation
- Navigated to the cloned Git repository.
- Checked the README file, which did not contain the password.
- Listed all local and remote Git branches.
- Switched to the `dev` branch.
- Inspected the commit history using `git log -p`.
- Found the password exposed in a commit on the development branch.

<img width="454" height="635" alt="image" src="https://github.com/user-attachments/assets/cc9f4e9e-5b6d-4738-8b9a-ab89da581afd" />

<img width="711" height="380" alt="image" src="https://github.com/user-attachments/assets/b4dfc1a2-73f7-4d40-bd66-cf6c81759db0" />


## Password
q93oex3VLz5MDG1n9lYowTv4Q8l7CDZL

## What I Learned
- How to list and switch between Git branches
- That sensitive data can exist in non-default branches
- Why all branches must be reviewed before publishing a repository
