# Password level 16

<img width="1340" height="537" alt="image" src="https://github.com/user-attachments/assets/ebba6dea-f23c-48bf-b473-f899a0b489c8" />

This level is similar to the previous one, but the service now expects the data to be sent over an encrypted connection using `SSL/TLS`.

and we use `openssl s_client` which is a command-line tool that lets us connect to an SSL/TLS-enabled service and send data securely,it works like `netcat` but with encryption.



<img width="457" height="75" alt="image" src="https://github.com/user-attachments/assets/1a454a9e-5179-497e-9343-6e507c10bedc" />

Here the  `openssl s_client` connects to the local server on port 30001 using SSL/TLS and sends that data securely. The server then replies with the next password.
