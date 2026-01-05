# Password for level 33

<img width="647" height="336" alt="level 32-33 qn" src="https://github.com/user-attachments/assets/37630548-2921-450d-9d66-c6e3aac20b06" />

Firsts less try to access level 32


<img width="1130" height="561" alt="level 32-33 step1" src="https://github.com/user-attachments/assets/16edbcb1-72f8-4fc4-b0d4-325cb321040d" />

if its `sh` shell then use `-t sh` in ssh command

<img width="437" height="170" alt="level 32-33 step 2" src="https://github.com/user-attachments/assets/ee39bde6-23ba-46a1-8641-2e1104188bb5" />

well its obivious what happens here, we cant basically type commands ...well as far as you noticed all commands that we use are in small letters and linux is  case sensitive, (LS is not ls for linux)

<img width="397" height="52" alt="level 32-33 step3" src="https://github.com/user-attachments/assets/a0bb9e65-134d-4c32-8bba-74740a2ca4bf" />

see!!!! so theres no way to type command in this shell....but what if we try to use another shell??which will break us out of this shell

(I REALLY URGE YOU TO MANUALLY TRY TO FIND OUT THE SOLUTION GOOGLE THE TOOLS NOT THE SOLUTIONS...ONLY COME BACK HERE IF THERES NO OTHER WAY!!!!)



<img width="863" height="257" alt="level 32-33 step4" src="https://github.com/user-attachments/assets/de5c9d70-fc79-4bac-9ec9-ae0a2318cb4e" />

A shell does not execute the text you type directly. It first performs expansions, such as replacing $HOME or $0 with their actual values, and only then runs the resulting command.

`$0` is a special shell variable that represents the name of the current shell or script,It is handled internally by the shell itself, not looked up as a command you typed

so when we type `$0` it  Expands `$0` to its own executable name , Executes that program, Starts a new, unrestricted shell

<img width="386" height="56" alt="image" src="https://github.com/user-attachments/assets/a95b27dd-0ca2-42fd-b0c1-c4389c23ca87" />

and thats it password for next level
