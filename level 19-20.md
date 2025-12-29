# Password for level 20

<img width="1572" height="345" alt="level 19-20 qn" src="https://github.com/user-attachments/assets/6e8e0b37-a317-4a54-bc01-c0882575e6bf" />

In this level we have to find password for user `bandit20` by using the setuid binary file in home directory of `bandit19` user.

`setuid` is a permission bit that makes a program run with the file owner’s privileges instead of the user who runs it. Here the program gets elevated permission not the user.




<img width="790" height="52" alt="level 19-20 step2" src="https://github.com/user-attachments/assets/d68064b9-9174-4609-8aa0-338672335570" />

In the above picture, the s indicates that the setuid bit is enabled.
This means the program will run with the file owner’s privileges, while any user who has execute permission on the file is allowed to run it.

<img width="517" height="108" alt="level 19-20 step3" src="https://github.com/user-attachments/assets/758ec569-d259-42da-85fa-b66753324071" />

The above picture clearly defines whats happening , we can see the program runs with  `bandit20` user's privilages.

NOTE!!! `bandit19` does not receive elevated privileges; only the program executes with `bandit20’s` permissions.

<img width="837" height="101" alt="level 19-20 sol" src="https://github.com/user-attachments/assets/90caa509-7cb0-42bb-ae7e-5462eb287a82" />


