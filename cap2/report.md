# Bug Bounty 

## URL 1: www.hackthissite.org

In this site i have registered with my email addressand logged in.

what i have found in this site is that we can do the basic challenges doing bug bounties.

### level one of the basic challenge 

![basic1](image.png)

![basic1](/assets/Screenshot%20from%202024-05-28%2021-51-31.png)

In the above picture it shows the source code of the challenge which contains the password for this challenge.

![basic1](/assets/Screenshot%20from%202024-05-28%2021-52-22.png)

### level two of the basic challenge

![basic2](/assets/Screenshot%20from%202024-05-28%2021-55-15.png)

Here as we can see the instructions says that sam forgot to upload the password file it means that there is no password for this challenge.

### level three of the basic challenge

![alt text](image-1.png)

![basic3](/assets/Screenshot%20from%202024-05-28%2021-56-59.png)

To see if we get any information from the source code of this file we checked it and found a hidden input which is stored in password.php so we went into the password.php directory from the url.

![basic3](/assets/Screenshot%20from%202024-05-28%2021-57-26.png)

Going to password.php we found the password for this challenge.

### level four of the basic challenge

In this challenge we are going to change where the password is being sent to.

![basic4](/assets/Screenshot%20from%202024-05-28%2021-58-25.png)

Going to inspect page of this site we can change the email to my email which the password is being sent to.
![basic4](/assets/Screenshot%20from%202024-05-28%2022-00-36.png)
![basic4](/assets/Screenshot%20from%202024-05-28%2022-01-50.png)

