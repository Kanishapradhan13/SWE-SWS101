In this cap we are given an ip address and asked to perform scans and vulnerability tests for the target IP address. 

So to start with I first searched the IP address on a browser and the instruction asked to hack into this server and gain root shell.

The first scan i did was a simple nmap scan 

> sudo nmap -O 10.3.21.140 

Here we gave root access to do the nmap OS scan.Doing this we found that there are two open ports in this server.

- 22/tcp open ssh
- 80/tcp open http  

![os scan](assets/img/OS%20scan.png)

Next we did a nmap scan to detect the version of the services running on the target.

> sudo nmap -sV 10.3.21.140 

Here we found the version of the services on the open ports.

- 22/tcp   open   ssh          OpenSSH 4.7p1 Debian 8ubuntu1 (protocol 2.0)
- 80/tcp   open   http         Apache httpd 2.2.8 ((Ubuntu) DAV/2)

We also did a level two verbosity scan to get more information for us.

![level2verbo](assets/img/level2verbo.png)

We did a port scan for both the open ports just to see if we get any more info but that didnt give us any new information. 

![portscan](assets/img/portscan.png)

![ports](assets/img/ports.png)

![ffuf](assets/img/ffuf.png)

![mysql](assets/img/mysql.png)

![users](assets/img/users.png)

![crackhash](assets/img/crackhash.png)


