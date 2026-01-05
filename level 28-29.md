# Password for level 29

<img width="1545" height="517" alt="level 28-29 qn" src="https://github.com/user-attachments/assets/fd135b11-b064-407a-a57f-5a4aa4bad2ee" />

The steps to clone this repo is same as before...we use `git clone` and dont forget the PORT!!!!!!!!

<img width="560" height="307" alt="level 28-29 step2" src="https://github.com/user-attachments/assets/5c048e28-48e6-4e41-ae92-352c05712abc" />

Here we expect to see the credentials for `level 29` but it has been removed!!!!

And remeber what i said about git in previous level....thats it!! It tracks changes and keeps a history of what and when change in a file , but it doesnt track changes automatically... it only tracks these changes when they are committed.
A commit is a snapshot of the project that Git saves intentionally by `YOU`, allowing you to track, review, and restore changes over time and a standard procedure is to `commit` changes made during production.

so what we can try to do is go back to previous commits and check the files.

<img width="1178" height="415" alt="level 28-29 step3" src="https://github.com/user-attachments/assets/b85c5849-119b-483e-ae98-f15f7630442e" />

with `git log` we can see previous commits and we do understand from the messages that they accidently leaked password in previous commit and it was fixed in the latest(current) commit all we need to do is check that previous commit
<img width="325" height="113" alt="image" src="https://github.com/user-attachments/assets/b94158aa-6bde-4151-9489-23537571a670" />

