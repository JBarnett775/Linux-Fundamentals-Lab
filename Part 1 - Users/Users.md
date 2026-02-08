# Users
## This part of my project is where I learnt the different commands around users that can used in Linux.

## Listing users
#### First of all I used the 'cat' comand to list all the current users
```
cat /etc/passwd
```
![Listing Users](images/Listing_users.png)

## Creating users
#### Next I wanted to add a couple of users, I did so using the 'sudo adduser' command. During this process I also had to give both of them a password.
```
sudo adduser alice
sudo adduser bob
```
#### Now if I re-run the commmand to list users we can see that Alice and Bob are now there.
![Listing Users Bob and Alice](images/listing_users_BA.png)


## Removing users
#### I can do this by using the following command
```
sudo userdel -r alice
``` 
![Listing Users](images/delete_user.png)

## Changing users
#### Now that I have created two new users I can now log into to one of them.
```
su - bob
```
 
#### As can be seen I am now logged in as 'bob', I can then use the logout command to log out of a user.
![Changing Users](images/changing_users.png)


## Creating groups
#### lets say I want to Bob and Alice to a group called 'accountants', I would use the following command
```
sudo groupadd accountants
cat /etc/group
```
#### We can now see that 'accountants' is now a listed group
![Listing Groups](images/listing_groups.png)


## Adding users to a group
#### Now that we have the accountants group set us, lets add Alice and Bob to it with the following command
```
sudo gpasswd -a bob accountants
sudo gpasswd -a alice accountants
```
![accountants users ](images/accoutants_users.png)
![adding users to group](images/adding_users_to_groups.png)

## This is the end of part 1, in part two I move onto learn how to manage permissions in Linux


















