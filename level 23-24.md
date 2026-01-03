# Password for level 24

<img width="1556" height="472" alt="level 23-24 qn" src="https://github.com/user-attachments/assets/74f67d55-51dd-4671-aba2-455232323332" />

Same as before a cronjob is running at a scheduled time, if we look into the running script.

in order to avoid permission issues we create a temporary directory by running `mktemp -d` command

All other steps are then done inside this temporary directory

<img width="870" height="440" alt="level 23-24 step1" src="https://github.com/user-attachments/assets/b18e5ccc-d065-4724-8893-954fe03a8b6e" />

we can see it executes and deletes all script in the mentioned directory

But not only that it also mentions that if the script user is bandit23 then it waits for one minute then executes and deletes the script

So here we have to create our first shell script in the `temp directory`


<img width="797" height="92" alt="level 23-24 step2" src="https://github.com/user-attachments/assets/b8fdb18a-0658-42c6-abc0-0f9acc0571ae" />

This is the script that we made from the image we can easily understand that it copies the password for level 24 and store it in a file `bandit24pass` we need to create it inside manually before running the script.

<img width="735" height="37" alt="level 23-24 step3" src="https://github.com/user-attachments/assets/e5e88a5b-870b-403b-b848-ad202f3d1d0a" />

then after giving executable permission we cp the script that we created to thae directory

<img width="927" height="21" alt="level 23-24 step4" src="https://github.com/user-attachments/assets/930a5491-defc-49bd-977d-463fc8cf220d" />

and we wait for a minute then check the `bandit24pass` its size will change from `0` to some value meaning the password has been copied into that file by running our script

<img width="848" height="341" alt="level 23-24 step 5" src="https://github.com/user-attachments/assets/50b8dac4-b8da-49d3-bbce-58f71d401ee6" />

Then we just `cat` into the file and there we have it...PASSWORD FOR LEVEL 24!!!!!

IF YOU DONE IT BY YOURSELFFF THEN GOOD JOB....YOU RE BECOMING BETTER!!!!
