# Level 22 → Level 23

## Objective
Find the password for Bandit Level 23 by analyzing a cron job that uses a predictable filename.

## Commands Used
ls /etc/cron.d  
cat /etc/cron.d/cronjob_bandit23  
cat /usr/bin/cronjob_bandit23.sh  
echo I am user bandit23 | md5sum | cut -d ' ' -f 1  
cat /tmp/8ca319486bfbc3663ea0fbe81326349

## Explanation
- Listed cron jobs in `/etc/cron.d`.
- Found the cron job `cronjob_bandit23`.
- Inspected the cron job to identify the executed script.
- Viewed the script `/usr/bin/cronjob_bandit23.sh`.
- Observed that the script generates a filename using an MD5 hash of a fixed string.
- Recreated the hash using `md5sum`.
- Used the generated hash to locate the file in `/tmp`.
- Read the file to obtain the password for Bandit Level 23.

<img width="1606" height="362" alt="image" src="https://github.com/user-attachments/assets/5f836d44-79a6-41fc-a425-71e69f346ed9" />


## Password
0Zf11ioIjMVN551jX3CmStKLYqjk54Ga

## What I Learned
- How predictable hashes can be exploited
- How MD5 hashing works in scripts
- How cron jobs can leak sensitive information
