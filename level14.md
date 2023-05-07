                     _                     _ _ _
                    | |__   __ _ _ __   __| (_) |_
                    | '_ \ / _` | '_ \ / _` | | __|
                    | |_) | (_| | | | | (_| | | |_
                    |_.__/ \__,_|_| |_|\__,_|_|\__|  



# LEVEL 13

## Level Goal:

The password for the next level can be retrieved by submitting the password of the current level to *port 30000 on localhost*


## Level information:

| port |             host               |
|-----:|--------------------------------|
| 2220 |  bandit.labs.overthewire.org   |

| Level14  |    Password                           |
|-------:  |---------------------------------------|
| Bandit14 |     4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e  |

## Commands you may need to solve this level

```
telnet
```

## Step-by-step solutions:

+ *Log into the game* 
 Use this following code to enter the game=>
```
ssh bandit14@bandit.labs.overthewire.org -p 2220
```
<sub>We have to enter ssh following the host and the port which is 2220 to enter the level  with banditN°level@host -p (port)</sub>

+ *Enter the password required* : 
```
4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
```
<sub>We found it during the previous level</sub>

+Once we entered the game we will *match the password* for the next level. 



 
``` 
 telnet localhost 30000

```
<sub> we  establish a Telnet session with a service or program running on the local machine that is listening on port 30000</sub>
```
Trying 127.0.0.1...
Connected to localhost.
Escape character is '^]'.
4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
Correct!
BfMYroe26WYalil77FoDi9qh59eK5xNr

```




+ *Exit the level to move to the next level*
```
exit

```
<sub>Login to the next level to find how to beat it</sub>

```
 ssh bandit15@bandit.labs.overthewire.org -p 2220

```
```
==============================================
|         N E X T      L E V E L             | ===>
==============================================    
```
