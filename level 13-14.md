# Password for level 14

<img width="1595" height="526" alt="level 13-14 qn" src="https://github.com/user-attachments/assets/35e38f2b-dd0c-4123-8def-df1077359e93" />

Here password file for level 14 can only be accessed by user `bandit14` , but we are logged as user `bandit13`, but we are given an `SSH private key` that can be used to log in to the next level,
`SSH private key` files are used for `passwordless` login. If you have the private key, you can log in to the server without typing a password, because the server checks it against the public key it already trusts.

<img width="472" height="93" alt="level 13-14 step1" src="https://github.com/user-attachments/assets/c2f0eab0-e6f5-4d32-ad22-dbda72aaf376" />

We can transfer this file to our local system using `scp` command,scp uses SSH for authentication and encryption, so files are transferred securely in the same way we log in using SSH.
All we need here is to specify the path of the file inside server and the path to a directory in local machine which we wish to store that file

<img width="313" height="47" alt="level 13-14 step2" src="https://github.com/user-attachments/assets/c37a5a48-3cb2-4824-bc50-1ac592f6fc43" />
<img width="1836" height="366" alt="level 13-14 step4" src="https://github.com/user-attachments/assets/e791fda3-cbdb-4242-95a5-3066a5fd8d48" />
In the above image we see the ssh.private key has been tranferred to our local system using `scp`.
Now we just need to SSH into the server as user `bandit14` using the given private key. Before doing that, we must set proper permissions on the key file so that only the owner can read it; otherwise the key is considered insecure, and SSH will refuse to use it
<img width="1192" height="621" alt="level 13-14 step5" src="https://github.com/user-attachments/assets/7fa40a2e-098d-4164-90f0-5bd65383802e" />

And since we logged in as user `Bandit14` we can obtain the password

<img width="607" height="57" alt="level 13-14 sol" src="https://github.com/user-attachments/assets/7734ff49-94e5-4dff-b44c-0a72e8e15908" />

<br>
<br>


IMPORTANT!!!!! Whats matters here is the contents inside the ssh file.

<br>

<img width="653" height="47" alt="image" src="https://github.com/user-attachments/assets/7f2217eb-c9ae-42a2-b57c-9af05b9ce1ee" />


we can copy the contents in the private keyfile and paste it in a file inside our local machine and by setting appropriate permissions, we can login  using same steps as before

<img width="472" height="50" alt="alternate sol step2" src="https://github.com/user-attachments/assets/f2639dd7-f72e-41ec-8d44-70572822f1ce" />
<img width="880" height="701" alt="alternate sol step 3" src="https://github.com/user-attachments/assets/e5a060c0-8c7d-4aba-9d3d-3f6d9bcb476d" />
<img width="1135" height="721" alt="alternate sol sol" src="https://github.com/user-attachments/assets/78746be9-158f-4ddd-a63b-65ba52cd2d6c" />

