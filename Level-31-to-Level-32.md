# Level 31 → Level 32

## Objective
Obtain the password for Bandit Level 32 by modifying a Git repository and pushing the required content.

## Commands Used
cd /tmp  
mkdir bandit31  
cd bandit31  
git clone ssh://bandit31-git@bandit.labs.overthewire.org:2220/home/bandit31-git/repo  
cd repo  
ls  
cat README.md  
echo "May I come in?" > key.txt  
git add .  
git config --global user.name "bandit"  
git config --global user.email "bandit@localhost"  
git commit -m "add key"  
git push origin master  

## Explanation
- Created a working directory in `/tmp`.
- Cloned the Bandit Level 31 Git repository.
- Read the `README.md` to understand the task.
- Created a file `key.txt` with the required content.
- Added the file to the Git staging area.
- Configured Git username and email for committing.
- Committed the changes to the repository.
- Pushed the commit to the remote repository.
- The server validated the submission and returned the password.

<img width="744" height="778" alt="image" src="https://github.com/user-attachments/assets/08687224-df83-41e6-818b-4acd08fb4950" />
<img width="689" height="728" alt="image" src="https://github.com/user-attachments/assets/8db305d8-1388-4071-910a-899696025fb1" />
<img width="515" height="528" alt="image" src="https://github.com/user-attachments/assets/68c17c05-1048-4d5e-8399-95bb50a5874e" />


## Password
309RfhqyALVBEZpvb6LYStshZoqo5sK

## What I Learned
- How to add, commit, and push changes to a Git repository
- How Git can be used as an authentication or challenge mechanism
- Why proper commit configuration is necessary
