# Password for level 32

<img width="1572" height="432" alt="level 31-32 qn" src="https://github.com/user-attachments/assets/54c6146a-55a9-424d-a1cd-1c56413a9444" />

Clone the repo

<img width="842" height="240" alt="level 31-32 step1" src="https://github.com/user-attachments/assets/18b119d5-68b8-47a8-9c70-dbcc31b7a8a5" />

So now we reach the part where we push (in other words, upload) a Git project to a remote repository such as GitHub. Pushing sends our committed changes from the local repository to the remote one so others can clone it like you been doing for past levels

<img width="911" height="276" alt="level 31-32 step2" src="https://github.com/user-attachments/assets/b29109fe-8193-48ea-863e-81960b914f4e" />

when we try to commit directly we are dealt with error because of `.gitignore` files ,there are some files  that we do not want to push on our repository maybe because its contains sensitive infomation or large files that we dont want in out remote repo 
so all we need to do is either force it or remove the `*.txt` from .gitignore `*.txt`means all files ending with .txt. and finally use `git commit` and `git push`

<img width="436" height="42" alt="image" src="https://github.com/user-attachments/assets/8a6cbdba-3a99-46d8-aa7a-37ad9ed3ba38" />
