                     _                     _ _ _
                    | |__   __ _ _ __   __| (_) |_
                    | '_ \ / _` | '_ \ / _` | | __|
                    | |_) | (_| | | | | (_| | | |_
                    |_.__/ \__,_|_| |_|\__,_|_|\__|  



# LEVEL 13

## Level Goal:

The password for the next level is stored  in */etc/bandit_pass/bandit14* and can only be *read by user bandit14*. 
For this level, you don’t get the next password, but you get a *private SSH key* that can be used to l*og into the next level*.
Note: localhost is a hostname that refers to the machine you are working on



## Level information:

| port |             host               |
|-----:|--------------------------------|
| 2220 |  bandit.labs.overthewire.org   |

| Level13  |    Password                           |
|-------:  |---------------------------------------|
| Bandit13 |     wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw  |

## Commands you may need to solve this level

```
ls 
ssh
cat
```

## Step-by-step solutions:

+ *Log into the game* 
 Use this following code to enter the game=>
```
ssh bandit13@bandit.labs.overthewire.org -p 2220
```
<sub>We have to enter ssh following the host and the port which is 2220 to enter the level  with banditN°level@host -p (port)</sub>

+ *Enter the password required* : 
```
wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw
```
<sub>We found it during the previous level</sub>

+Once we entered the game we will *search the s the password* for the next level. 
We will use the commands  `ls` and `ssh ` to write this statement


=> Show all the files 
``` 
 ls -a

```
```
.  ..  .bash_logout  .bashrc   .profile  sshkey.private
```

=>`ssh -i` :used to specify the identity (private key) file to be used for authentication when connecting to an SSH server


```
ssh -i sshkey.private bandit14@localhost
``` 
<sub>localhost: hostname that refers to the machine you are working on</sub>


```
Are you sure you want to continue connecting (yes/no)? yes

```
=> Now , we are inside Bandit14 , we have to get the password from */etc/bandit_pass/bandit14*
```
cat /etc/bandit_pass/bandit14
```

```
4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
```


+ *Exit the level to move to the next level*
```
exit

```
<sub>Login to the next level to find how to beat it</sub>

```
 ssh bandit14@bandit.labs.overthewire.org -p 2220

```
```
==============================================
|         N E X T      L E V E L             | ===>
==============================================    
```
