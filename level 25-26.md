# Password for level 26

<img width="1542" height="491" alt="level 25-26 qn" src="https://github.com/user-attachments/assets/599ef245-4eb4-4cd5-b814-d542e9c013e8" />

When logging in as bandit25, you don’t get a normal command-line shell.
Instead, a program starts automatically.

In this case you need to know how linux program works:

If all the text the program returns fits on the screen → they exit immediately
If the text does not fit → they pause and wait for input

when you try to login as user bandit 25 you may thing that the connection got stuck when you dont see the command-line but actually its `more` s doing

Try to login as `bandit 25` with you terminal as small as possible and you il see something like below: 

<img width="700" height="100" alt="level 25-26 step2" src="https://github.com/user-attachments/assets/5c21fe0c-949b-4276-b1b7-6529ccf409a3" />

when you see something like this you can resize back to normal and you can also get the private sshkey for `bandit 26` 
<img width="500" height="400" alt="level 25-26 step1" src="https://github.com/user-attachments/assets/635686e2-09d1-4dfd-9df2-4894a9de7a92" />'

and thats it!!!!

But there s a better way with `:e` and when you nagivate to /etc/bandit_pass/bandit26 you can get password for `bandit 26`


 <img width="415" height="87" alt="level 25-26 sol" src="https://github.com/user-attachments/assets/96fc5cb6-3ef0-4857-b30e-eba1047d904a" />

 and its best to use bash so

<img width="297" height="83" alt="level 25-26 sol2" src="https://github.com/user-attachments/assets/67574209-d1a6-4b40-9893-15da8e45b4ff" />

and just by `:shell` you can enter as bandit 26
<img width="297" height="132" alt="level 25-26 final sol" src="https://github.com/user-attachments/assets/babaeb2c-7002-4b69-9079-c4f4d30d15f6" />
