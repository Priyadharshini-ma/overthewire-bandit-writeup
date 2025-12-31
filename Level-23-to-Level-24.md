# Level 23 → Level 24

## Objective
Find the password for Bandit Level 24 by exploiting a cron job that executes scripts placed in a writable directory.

## Commands Used
ls /etc/cron.d  
cat /etc/cron.d/cronjob_bandit24  
cat /usr/bin/cronjob_bandit24.sh  
cd /tmp  
rm -rf myscript  
mkdir myscript  
cd myscript  
nano getpass.sh  
chmod +x getpass.sh  
cat /tmp/bandit24_pass

## Explanation
- Listed cron jobs in `/etc/cron.d`.
- Found the cron job `cronjob_bandit24`.
- Inspected the cron script `/usr/bin/cronjob_bandit24.sh`.
- Observed that it executes scripts placed in a writable directory.
- Created a malicious script to copy the password to `/tmp`.
- Made the script executable so it could be run by cron.
- Waited for the cron job to execute.
- Read the output file to obtain the password.

<img width="1595" height="481" alt="image" src="https://github.com/user-attachments/assets/f1e247f8-d102-4c8a-85d9-1e66308160c7" />

a<img width="879" height="386" alt="image" src="https://github.com/user-attachments/assets/445a8188-80a4-4a38-ab7b-f4f8edc5e485" />


## Password
gb8KRRCsshuZXI0tUuR6ypOFjiZbf3G8

## What I Learned
- How insecure cron job configurations can be exploited
- Why writable directories should never be trusted in scheduled tasks
