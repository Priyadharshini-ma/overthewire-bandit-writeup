# Level 20 → Level 21

## Objective
Find the password for Bandit Level 21 by using a program that connects to a listening network service.

## Commands Used
nc -l 4444  
./suconnect 4444

## Explanation
- Started a listening service on port `4444` using `nc -l 4444`.
- In another terminal, executed the program `suconnect` with port `4444` as an argument.
- The `suconnect` program connected back to the listening service.
- Sent the password for Bandit Level 20 through the connection.
- The service responded with the password for Bandit Level 21.

<img width="464" height="85" alt="image" src="https://github.com/user-attachments/assets/c941028a-4e75-4475-9fb7-5890a157a946" />
<img width="561" height="81" alt="image" src="https://github.com/user-attachments/assets/f32ea5af-b443-4cd5-a33e-5fa2ff5ab7f3" />


## Password
EeoULMCra2q0dSkYj561DX7s1CpBuOBt

## What I Learned
- How to use `nc` (netcat) in listening mode
- How programs can communicate over network sockets
- How client–server interactions are used in CTF challenges
