# Level 32 → Level 33

## Objective

Obtain the password for the final Bandit level by escaping a restricted shell environment.

## Commands Used

$0
cat /etc/bandit_pass/bandit33

## Explanation

* Logged into Bandit Level 32 and encountered a restricted shell that prevented the execution of common commands.
* Executed `$0` to spawn the default shell associated with the current process.
* Successfully escaped the restricted environment and gained access to a normal shell.
* Read the password file for Bandit Level 33.

<img width="639" height="234" alt="image" src="https://github.com/user-attachments/assets/1af60e56-d49e-41e8-b6a0-5c7595a3ca39" />


## Password

tQdtbs5D5i2vJwkO8mEyYEyTL8izoeJ0

## What I Learned

* How restricted shells limit command execution
* How invoking `$0` can be used to escape poorly configured restricted shells
* The importance of securely configuring shell restrictions
