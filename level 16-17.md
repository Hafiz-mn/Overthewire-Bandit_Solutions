# Password for level 17

<img width="900" height="537" alt="level 16-17 qn" src="https://github.com/user-attachments/assets/0a2bf293-1c94-4168-a2f5-ff8d8ca8e780" />

In this level, we are given a range of ports (31000–32000) on localhost. Our first task is to identify which ports in this range are actually listening for connections. However, finding open ports alone is not enough. Among the listening ports some services accept plain text, some services require `SSL/TLS`-encrypted communication ,only one of the SSL-enabled services will accept the current level’s password and respond with the credentials for the next level.

In the previous level, we were given a specific port to which we could send the password directly. In this level, however, we are given a range of 1000 ports and must first find which port is actually relevant, manually connecting to each port and testing it one by one is inefficient and impractical.

So Here we can use `nmap` command line tool to search for open ports, where we can define the range of ports to be scanned 


<img width="600" height="221" alt="level 16-17 step 1" src="https://github.com/user-attachments/assets/fc1a6f95-282b-4cb4-835a-a5b179c84583" />


So here we found 5 open ports, now that made our work easier , now since its just a few ports we can find by sending the current password to each ports directly using `openssl s_clent` and the right one will return the credentials for next level. 

But what if the number of ports was much larger — say `100 or even 500 ports`? In that case, manually testing each port would not be a practical approach.
To handle this efficiently, we need a way to narrow down the ports based on the type of service they are running. Using the same `nmap` tool, we can go beyond simply checking whether a port is open and instead identify the service and protocol running on each port.

<img width="878" height="262" alt="level 16-17 step2" src="https://github.com/user-attachments/assets/f67e0582-e226-4009-a255-645edbbe0ab4" />
<br>
<br>


As we can see, there are 2 ports that are listening with SSL/TLS enabled. Other ports are using `echo` service they just returns the data that we sent them, one of the `SSL` ports `31518` is same as an `echo` service but wrapped in `SSL/TLS` encryption. So that just leaves the final port `31790`.

<img width="500" height="500" alt="level 16-17 sol" src="https://github.com/user-attachments/assets/62faf371-3a07-4127-a36e-6591d06e517a" />

And we are given with the private key for the next level 


