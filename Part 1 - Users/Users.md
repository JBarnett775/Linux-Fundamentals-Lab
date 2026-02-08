# Users
## This part of my project is where I learnt the different commands around users that can used in Linux.

## Listing users
#### First of all I used the 'cat' comand to list all the current users
```
cat /etc/passwd
```
insert image

## Creating users
#### Next I wanted to add a couple of users, I did so using the 'sudo adduser' command. During this process I also had to give both of them a password.
```
sudo adduser alice
sudo adduser bob
```
#### Now if I re-run the commmand to list users we can see that Alice and Bob are now there.
insert image

## Changing users
#### Now that I have created two new users I can now swap to one of them.
```
su - bob
```
insert image 
#### As can be seen I am now logged in as 'bob', I can then use the logout command to log out of a user.
insert image

