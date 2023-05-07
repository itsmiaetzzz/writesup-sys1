                     _                     _ _ _
                    | |__   __ _ _ __   __| (_) |_
                    | '_ \ / _` | '_ \ / _` | | __|
                    | |_) | (_| | | | | (_| | | |_
                    |_.__/ \__,_|_| |_|\__,_|_|\__|  



# LEVEL 8

## Level Goal:


The password for the next level is stored in the file *data.txt* and is the *only line of text that occurs only once*.

## Level information:

| port |             host               |
|-----:|--------------------------------|
| 2220 |  bandit.labs.overthewire.org   |

| Level8 |    Password                           |
|-------:|---------------------------------------|
| Bandit8|                                       |

## Commands you may need to solve this level

```
uniq , cat , ls 
```

## Step-by-step solutions:

+ *Log into the game* 
 Use this following code to enter the game=>
```
ssh bandit6@bandit.labs.overthewire.org -p 2220
```
<sub>We have to enter ssh following the host and the port which is 2220 to enter the level 2 with bandit2@host -p (port)</sub>

+ *Enter the password required* : 
```
P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU
```
<sub>We found it during the previous level</sub>

+Once we entered the game we will *search the file that contains the password* for the next level that is somewhere on the server .


We will use the find to write this statement

``` 

``` 


``` 

``` 

It shows us the file that correspond with the properties defined.
+We will enter this file and show the password.

``` 
 cd /var/lib/dpkg/info
``` 

``` 
cat  bandit7.password
```
<sub>
  cat :  concatenate files and print on the standard output
  cat will show the content of the file : for this game , it will show the password for the next level
</sub>


``` 


```

+ *Exit the level to move to the next level*
```
exit

```
<sub>Login to the next level to find how to beat it</sub>

```
 ssh bandit9@bandit.labs.overthewire.org -p 2220

```
```
==============================================
|         N E X T      L E V E L             | ===>
==============================================    
```
