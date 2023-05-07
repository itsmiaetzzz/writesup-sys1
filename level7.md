                     _                     _ _ _
                    | |__   __ _ _ __   __| (_) |_
                    | '_ \ / _` | '_ \ / _` | | __|
                    | |_) | (_| | | | | (_| | | |_
                    |_.__/ \__,_|_| |_|\__,_|_|\__|  



# LEVEL 7

## Level Goal:

-Find the password for the next level stored in the file *data.txt* next to *the word millionth* 




## Level information:

| port |             host               |
|-----:|--------------------------------|
| 2220 |  bandit.labs.overthewire.org   |

| Level 7|  Password                             |
|-------:|---------------------------------------|
| Bandit7|7 z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S   |

## Commands you may need to solve this level

```
grep
```

## Step-by-step solutions:

+ *Log into the game* 
 Use this following code to enter the game=>
```
ssh bandit7@bandit.labs.overthewire.org -p 2220
```
<sub>We have to enter ssh following the host and the port which is 2220 to enter the level 7 with bandit7@host -p (port)</sub>

+ *Enter the password required* : 
```
z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S
```
<sub>We found it during the previous level</sub>

+Once we entered the game we will *search the file that contains the password* for the next level that is *data.txt* next to *the word millionth* 


We will use the `grep` command to write this statement

``` 
grep "millionth" data.txt
``` 
<sub> `grep` is used to search for specifi  words in files.
  In this case, you can search for the word "millionth" in the "data.txt" file </sub>


``` 
millionth       TESKZC0XvTetK0S9xNwm25STk5iWrBvP

``` 
<sub>The password for the next the level is near the word "millionth"</sub>


+ *Exit the level to move to the next level*
```
exit

```
<sub>Login to the next level to find how to beat it</sub>

```
 ssh bandit8@bandit.labs.overthewire.org -p 2220

```
```
==============================================
|         N E X T      L E V E L             | ===>
==============================================    
```
