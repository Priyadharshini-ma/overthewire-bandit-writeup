# Level 15 → Level 16

## Objective
Find the password for Bandit Level 16 by communicating with an SSL-enabled service.

## Commands Used
ncat --ssl localhost 30001

## Explanation
- Connected to a local service running on port `30001` using `ncat` with SSL support.
- Submitted the password for Bandit Level 15 to the service.
- The service responded with the password for Bandit Level 16.

<img width="468" height="80" alt="image" src="https://github.com/user-attachments/assets/a6d1926c-5d6f-4f6e-82a4-dd8ad9d8a865" />


## Password
kSkvUpMQ7LBycM4GBPvCvT1BfWRy0Dx

## What I Learned
- Difference between plain `nc` and `ncat --ssl`
- How SSL/TLS can be used in network communication
- How services may require encrypted connections
