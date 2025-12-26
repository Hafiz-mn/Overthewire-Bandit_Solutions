# Password for level 13

<img width="1583" height="517" alt="level 12-13 qn" src="https://github.com/user-attachments/assets/c8a5d49b-af73-4600-a327-90f97754f31a" />

Here we are given a hexdump of a file, but not only that, it also has been compressed many times.

So if we try to read the contents in the file now, it could look like this.




<img width="400" height="400" alt="level 12 -13 step1" src="https://github.com/user-attachments/assets/3a156adc-528b-4dbe-b668-ed83a6cef248" />


We might have to create multiple files with different names that might make home directory look confusing and messy so we use `mktemp -d` to create a directory for the messy stuff. 

We will use `xxd` command which can create hex dump or reverse from hex dump .

<img width="866" height="53" alt="level 12-13 step2 " src="https://github.com/user-attachments/assets/f331f391-307b-4bab-8fa4-cb356658dad9" />

And by using `file` we can find the file type here we see its gzip compressed

<img width="922" height="67" alt="level 12-13 step3" src="https://github.com/user-attachments/assets/e60b50c5-c3e7-4d83-85da-7b163afb65da" />

So we have to decompress it using `gzip`, `gzip` only works in files in `.gz` format so we need to rename it, what matters here is that in the end it should have `.gz`
then we get a bzip2 file which requires the format of `.bz2` and then theres tar .
<img width="685" height="50" alt="level 12-13 step4" src="https://github.com/user-attachments/assets/3a12a006-d972-4d03-abbc-c4bdac13f7a9" />
<img width="857" height="18" alt="level 12 -13 step5" src="https://github.com/user-attachments/assets/189b99bf-3571-4de5-93e8-cd89d81c3068" />



we il get different files after each decompression and finally will get a text file.


