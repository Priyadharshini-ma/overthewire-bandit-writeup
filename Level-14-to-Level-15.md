# Level 14 → Level 15

## Objective
Find the password for Bandit Level 15 by submitting the current level’s password to a local service.

## Commands Used
nc localhost 30000

## Explanation
- Connected to a local TCP service running on port `30000` using `nc` (netcat).
- Sent the password for Bandit Level 14 to the service.
- The service responded with the password for Bandit Level 15.

<img width="382" height="83" alt="image" src="https://github.com/user-attachments/assets/c73fe245-0335-44a0-b2b7-4ec06a94847c" />


## Password
8xCjmgokBGLhHFZLGE5Tmu4M2tKJQo

## What I Learned
- How to use `nc` (netcat) to communicate with network services
- How local services can be used in CTF challenges
