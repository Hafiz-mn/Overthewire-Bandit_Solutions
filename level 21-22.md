# Password for Level 22

<img width="1523" height="385" alt="level 21-22 qn" src="https://github.com/user-attachments/assets/8e2be248-0fd4-4cc8-9163-b688e4274581" />

In this level there s a cronjob that executes a command at a fixed period of time and it is related to the password for the next level. 

When we look at the cronjob we see a bash script being executed,

<img width="1141" height="201" alt="level 21-22 step 1" src="https://github.com/user-attachments/assets/37587285-5f5f-4687-817e-353b296735b7" />

When we take a look inside the bash script using `cat` , we see a file being created inside `/tmp` and also after that the password for level 22 
is stored inside that file , so all we need to do is read the file contents

and there we have it the password for the next level!!!!!

<img width="835" height="203" alt="level 21-22 sol" src="https://github.com/user-attachments/assets/9e505702-a0d3-4303-a0ce-bfa8333889ec" />
