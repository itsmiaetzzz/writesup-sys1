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

+  I connect to the localhost server with the OpenSSL client and send the password from this level


```
bandit15@bandit:~$ openssl s_client -connect localhost:30001
BfMYroe26WYalil77FoDi9qh59eK5xNr
Correct!
cluFn7wTiGryunymYOu4RcffSxQluehd
```
<sub> The server then sends back the password for the next level. </sub>


+  Once we have  *the password* for the next level , we can continue to the next level. 



```
==============================================
|         N E X T      L E V E L             | ===>
==============================================    
```
