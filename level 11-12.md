# Password for level 12

<img width="1250" height="442" alt="level 11-12 qn" src="https://github.com/user-attachments/assets/2bc04617-bd91-406d-9382-72fae0a66943" />

In this level we're give a `data.txt` in which each letter is replaced by their 13th alphabet respectively,
So `A and a` becomes `N and n`, similarly for other characters.

<img width="655" height="141" alt="level 11-12 step1" src="https://github.com/user-attachments/assets/4c95f123-49f8-4a54-8e67-7e43342f72f3" />





Here we use `tr`(use man for more details)


<img width="465" height="55" alt="level 11-12 sol" src="https://github.com/user-attachments/assets/494d5849-2c26-4bf9-b790-66e3748dc9c5" />



What the command basically does is that it takes the output of `cat` and returns password by translating characters one-to-one: each letter in A–Z a–z is replaced by the letter in the same position in N–Z A–M n–z a–m, so every character is shifted 13 places with wrap-around.
