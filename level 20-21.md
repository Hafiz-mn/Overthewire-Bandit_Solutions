# Password for level 21

<img width="1553" height="432" alt="level 20-21 qn" src="https://github.com/user-attachments/assets/373015d7-6638-4285-9147-9a454f267712" />

In this level, a setuid binary running as bandit20 connects to a user-specified local port, verifies the previous level’s password, and returns the password for the next level if the verification succeed
But there isnt a service thats assigned on a port which provides the password for `bandit20`, so we need to find a free port and make it listen for a connection to establish and sents the password for comaprison

<img width="945" height="397" alt="level 20-21 sol" src="https://github.com/user-attachments/assets/385a5a21-8b33-404d-a8c4-5501f72057f0" />

`tmux` is a tool that allows us to create multiple terminals within the same SSH session.
In this level, we need two processes to run at the same time:
one is the `setuid binary`, which connects to a specified local port, and the other is an nc (netcat) service, which listens on that port and sends the password for verification.

NOTE!!! Here any free port can be assigned
