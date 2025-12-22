# Password for level 6

<img width="1072" height="422" alt="level 5 to 6 qn" src="https://github.com/user-attachments/assets/b4f44030-5293-4cab-ac8e-6abffa34583f" />

In this Level the password is stored in a file inside `inhere` directory that has some given properties.

<img width="1195" height="171" alt="level 5 to 6 step 1" src="https://github.com/user-attachments/assets/3515c4e9-de11-427a-8108-53948f0d9daa" />

When we check the `inhere` directory, it contains many subdirectories and files. Manually opening each file to find the correct one is inefficient and time-consuming and not the smartest way.

So we have to use command-line tools to narrow down the correct file automatically.

Here we combine two commands using pipelining `|`, we know by using `ls` we can list file contents inside a directory, by using `-l` we get more detailed information of the listed files including size and to list contents of multiple directory we use `./*` where `.` represents current directory and `*` means 'everything in the directory.

We can use `grep` command to print lines that matches a pattern that we give, since the file size is `1033 bytes`,we can use that to narrow down.

So by combining two commands `ls ./* -al | grep 1033` we narrow down the files


<img width="643" height="56" alt="level 5 to 6 step 2" src="https://github.com/user-attachments/assets/a552d942-ae18-4702-878e-558b0c43d18e" />

The file .file2 has permissions -rw-r-----, where r stands for read and w stands for write. Since there is no x permission set, the file is not executable and can only be read or modified by authorized users.
We have got the file but we have yet to find its location , for that we use `find` tool.
<img width="1195" height="47" alt="level 5 to 6 step 3 " src="https://github.com/user-attachments/assets/a41dbb7d-d617-4d1f-bb81-d483e1329bfb" />

And finally use `cat` to obtain the password

<img width="858" height="62" alt="image" src="https://github.com/user-attachments/assets/d88c6e71-13b3-40c9-aec9-f6540defe80c" />


