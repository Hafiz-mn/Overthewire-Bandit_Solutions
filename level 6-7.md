# Password for Level 7

<img width="943" height="432" alt="level 6 to 7 qn" src="https://github.com/user-attachments/assets/08b0af7d-96eb-44f9-a664-ce9ed64a96db" />

This level is little different from other levels, here the password is stored somewhere in the server, we are not given any specific directory.
and the conditions are also different, its owned by user `bandit7` and group `bandit6`.

To handle this efficiently, we can use the `find` command with appropriate options. To check which options are available, we can refer to the manual using `man find` or view a quick summary with `find --help`.


<img width="1003" height="625" alt="Screenshot 2025-12-21 165122" src="https://github.com/user-attachments/assets/5713e916-4354-4e0f-bfd4-b12c7f29ac1f" />

Since the file can be located anywhere on the server, we start searching from the root directory (/). `/` is the top-level directory every file and directory on the system exists under `/`.

We will hit many directories where we don’t have permission to read. so we use `2>dev/null` 2 is the standard error which is redirected to `/dev/null` - a special file that discards anything sent to it.

<img width="943" height="49" alt="level 6 to 7 step 2" src="https://github.com/user-attachments/assets/d7ee6eb4-4582-43e7-a160-e09d770dec6f" />

and it returns the matching files.
<img width="977" height="47" alt="level 6 to 7 step 3" src="https://github.com/user-attachments/assets/b96224ff-107b-40cd-8c66-c533b395733b" />

<img width="852" height="63" alt="image" src="https://github.com/user-attachments/assets/732d3a04-bc15-4a9a-b79e-11e6a1573334" />


