# Bug Bounty 

## URL 1: www.hackthissite.org

In this site i have registered with my email addressand logged in.

what i have found in this site is that we can do the basic challenges doing bug bounties.

### level one of the basic challenge 

![basic1](/assets/image.png)

![basic1](/assets/Screenshot%20from%202024-05-28%2021-51-31.png)

In the above picture it shows the source code of the challenge which contains the password for this challenge.

![basic1](/assets/Screenshot%20from%202024-05-28%2021-52-22.png)

### level two of the basic challenge

![basic2](/assets/Screenshot%20from%202024-05-28%2021-55-15.png)

Here as we can see the instructions says that sam forgot to upload the password file it means that there is no password for this challenge.

### level three of the basic challenge

![alt text](/assets/image-1.png)

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

![basic4](/assets/Screenshot%20from%202024-05-28%2022-02-13.png)

I have recieved the password in my email 

![basic4](/assets/Screenshot%20from%202024-05-28%2022-04-57.png)

### level five of the basic challenge

Similar to the previous challenge we changed the email where the password is being sent to from the inspect form.

![basic5](/assets/Screenshot%20from%202024-05-28%2022-04-02.png)

![basic5](/assets/Screenshot%20from%202024-05-28%2022-04-42.png)

![basic5](/assets/Screenshot%20from%202024-05-28%2022-05-47.png)

### level six of the basic challenge

First we tried to check what the encryption method is used here so we tried to encrypt 12345 for which we got the answer 13579

Here we can see a pattern where the pasword is being incremented by 1 each time we go further like 
- the first number remains the same 
- the second number is incremented by 1
- the third number is being incremented by 2 and so on.

So applying this concept of the given encrypted password i decremented it one by one 

To do that i used the ascii table to check for the values before a semicolon 

![basic6](image-1.png)

The encrypted code is 4652b6da

![basic6](image.png)

![basic7](image-2.png)

### level 7 of the basic challenge

Here we inserted an injection and we get an php file url which we can use to get the password.

![basic7](/assets/Screenshot%20from%202024-05-30%2020-37-05.png)

![basic7](/assets/Screenshot%20from%202024-05-30%2020-39-12.png)

![basic7](/assets/Screenshot%20from%202024-05-30%2020-39-56.png)

![basic7](/assets/Screenshot%20from%202024-05-30%2020-42-23.png)

### level 8 of the basic challenge 

I tried an injection here again and from here we got the path to the php file containing the password.

![basic8](/assets/Screenshot%20from%202024-05-30%2020-45-40.png)

![basic8](/assets/Screenshot%20from%202024-05-30%2020-46-23.png)

![basic8](/assets/Screenshot%20from%202024-05-30%2020-47-10.png)

![basic8](/assets/Screenshot%20from%202024-05-30%2020-47-49.png)

### level 9 of the basic challenge
To do this we need to go back to challenge 8 and insert an injection with the level 9 reference in the injection. 

![basic9](/assets/Screenshot%20from%202024-05-30%2020-49-31.png)

We get a php file path and going to that path we get the password for this challenge

![basic9](/assets/Screenshot%20from%202024-05-30%2020-49-58.png)
![basic9](/assets/Screenshot%20from%202024-05-30%2020-51-02.png)

![basic9](/assets/Screenshot%20from%202024-05-30%2020-58-30.png)
## URL 2: 10.3.21.141:8008

In gruyere I created an account 
![cheese](/assets/Screenshot%20from%202024-05-30%2013-16-57.png)

### privilege elevation 

By inserting this query into the url we get admin access where we can delete accounts.

![cheese](/assets/Screenshot%20from%202024-05-30%2013-18-51.png)

We got the access to manage this server and add snipets
![cheese](/assets/Screenshot%20from%202024-05-30%2013-23-42.png)

![cheese](/assets/Screenshot%20from%202024-05-30%2013-28-07.png)

## URL 3: 10.3.21.141:8000

Here in this site i had already created an acccount so i tried an injection 

![pixi](/assets/Screenshot%20from%202024-05-30%2020-29-15.png)
