# Password for level 10

<img width="700" height="403" alt="level 9 to 10 qn" src="https://github.com/user-attachments/assets/92bfd9b8-06af-4d8b-990d-9e5ac2918ccf" />

In this level the data.txt file contains non-human readable strings which looks like below

<img width="700" height="916" alt="level 9 to 10 step 2" src="https://github.com/user-attachments/assets/bcb5ebc1-423f-4427-9497-e902693b1c67" />

And our password's in here somewhere
But we are also given that our password is preceeded by some `=` symbols for eg. "====ourpassword"

Since `cat` blindly outputs all file contents, it becomes ineffective when the file includes non-printable or binary data, making it difficult to identify meaningful information.

So to counter this we use `strings` command which will only return human readable strings.

<img width="512" height="366" alt="level 9 to 10 step 3" src="https://github.com/user-attachments/assets/22149f6e-0f98-475c-a56b-e5db5a024652" />


And by combining this with `grep` we get..thats right the password!!!.

<img width="400" height="145" alt="level 9 to 10 sol" src="https://github.com/user-attachments/assets/d66646f5-daf7-40f6-9f83-a7a9be1338ba" />
