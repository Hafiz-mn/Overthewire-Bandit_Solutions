# Password for level 23

<img width="1565" height="411" alt="level 22-23 qn" src="https://github.com/user-attachments/assets/b19ab734-584a-4584-9078-17dfa6d71f02" />

<br>
<br>

This level is same as the previous ones we need check the running cronjob which is related to password for level 23



<img width="700" height="392" alt="level 22-23 step1" src="https://github.com/user-attachments/assets/05f1c646-ec85-4926-a6d5-483f72d06b6e" />


and we see some commands ,some other variables in the script that is being executed

<br>
We can try to execute the commands manually to try to understand whats its doing
<br>
<br>

<img width="988" height="132" alt="level 22-23 step2" src="https://github.com/user-attachments/assets/749cad21-3454-4545-b003-c7b1af21aed2" />

and we see that its storing the password for given users in  `/tmp` directory , when we tried `bandit22` it gave password for current level password that we have found in previous levels
so to find `bandit23` password...we just replace `bandit22` with `bandit23`.


<img width="840" height="77" alt="level 22-23 sol" src="https://github.com/user-attachments/assets/c02bb691-6652-4176-918e-cb1e3adf2dfa" />


Out of curiosity i tried to find password for level 24 too...try it for yourself 
