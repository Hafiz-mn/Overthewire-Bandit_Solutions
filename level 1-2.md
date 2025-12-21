# Find password for level 2 

<img width="600" height="400" alt="level 2 qn" src="https://github.com/user-attachments/assets/a1b87070-942c-4be7-be5a-af6e2378716c" />

In this level we need to find password for level 2 which is in a file name `-`. At first glance we think it's a normal filename but issue is in Linux "-" is commonly used as a special option meaning "standard input" or a flag to specify an argument.
When you try to use commands like `cat -` or `ls -`, the system interprets `-` as an option, not as a filename.


To read the contents of `-`, you need to tell the system that `-` is a filename, not an option.
so we specify it by using `cat ./-` which tells the system to read the contents of file named `-` in the "current directory" or `cat -- -` which does the same.

And we have got the password for the next level.

<img width="469" height="300" alt="level 2 password" src="https://github.com/user-attachments/assets/240857a5-dd60-4bea-973a-d36e6cae89fe" />

