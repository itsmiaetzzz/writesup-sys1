                     _                     _ _ _
                    | |__   __ _ _ __   __| (_) |_
                    | '_ \ / _` | '_ \ / _` | | __|
                    | |_) | (_| | | | | (_| | | |_
                    |_.__/ \__,_|_| |_|\__,_|_|\__|  



# LEVEL 15

## Level Goal:

The password for the next level can be retrieved by submitting the password of 
the current level to *port 30001 on localhost *.




## Level information:

| port |             host               |
|-----:|--------------------------------|
| 2220 |  bandit.labs.overthewire.org   |

| Level15  |    Password                           |
|-------:  |---------------------------------------|
| Bandit15 |    BfMYroe26WYalil77FoDi9qh59eK5xNr   |

## Commands you may need to solve this level

```
 openssl, s_client
```

## Step-by-step solutions:

+ Find the password for bandit14* 
 Use this following code to enter the game=>
```
cat /etc/bandit_pass/bandit14
```
```
4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
```
<sub>we need to submit the password to port 30000 on localhost we used `nc` to connect to localhost port 3000 and write the password.</sub>


```
nc localhost 30000
4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
Correct!
BfMYroe26WYalil77FoDi9qh59eK5xNr
```

+Once we have  *the password* for the next level , we can continue to the next level. 



 
```
==============================================
|         N E X T      L E V E L             | ===>
==============================================    
```
