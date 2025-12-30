# Level 21 → Level 22

## Objective
Find the password for Bandit Level 22 by analyzing a cron job configuration.

## Commands Used
ls /etc/cron.d  
cat /etc/cron.d/cronjob_bandit22  
cat /usr/bin/cronjob_bandit22.sh  
cat /tmp/t70GldS9s0RqQh9aMcz6ShpAoZKF7fgv

## Explanation
- Listed cron job configurations in `/etc/cron.d`.
- Found a cron job named `cronjob_bandit22`.
- Viewed the cron job to identify the script being executed.
- Inspected the script `/usr/bin/cronjob_bandit22.sh`.
- The script writes the password to a file in `/tmp`.
- Read the generated file to obtain the password for Bandit Level 22.

<img width="1604" height="219" alt="image" src="https://github.com/user-attachments/assets/ee17efeb-b928-46ec-afdc-9c8091d2abee" />


## Password
tRae0UfB9v0UzbCdn9cY0gQnds9GF58Q

## What I Learned
- How cron jobs work in Linux
- How scheduled tasks can expose sensitive information
- How to trace cron jobs to the scripts they execute
