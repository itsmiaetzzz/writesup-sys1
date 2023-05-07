                     _                     _ _ _
                    | |__   __ _ _ __   __| (_) |_
                    | '_ \ / _` | '_ \ / _` | | __|
                    | |_) | (_| | | | | (_| | | |_
                    |_.__/ \__,_|_| |_|\__,_|_|\__|  



# LEVEL 8

## Level Goal:


The password for the next level is stored in the file *data.txt in one of the few human-readable strings*, *preceded by several ‘=’ characters*.



## Level information:

| port |             host               |
|-----:|--------------------------------|
| 2220 |  bandit.labs.overthewire.org   |

| Level9 |    Password                           |
|-------:|---------------------------------------|
| Bandit9 |  EN632PlfYiZbn3PhVK3XOGSlNInNE00tP    |

## Commands you may need to solve this level

```

```

## Step-by-step solutions:

+ *Log into the game* 
 Use this following code to enter the game=>
```
ssh bandit9@bandit.labs.overthewire.org -p 2220
```
<sub>We have to enter ssh following the host and the port which is 2220 to enter the level 9 with bandit9@host -p (port)</sub>

+ *Enter the password required* : 
```
EN632PlfYiZbn3PhVK3XOGSlNInNE00t
```
<sub>We found it during the previous level</sub>

+Once we entered the game we will *search the file that contains the password* for the next level 
We will use the find to write this statement



``` 
 grep  data.txt

```
<sub>
 `grep`: searches for lines

`data.txt` is the file to search in.

`<(...)` is a convenient syntax that allows you to manipulate the output of a command as if it were stored in a file, without the need to create an actual file on the file system.
</sub>
 
```

```
+ *Exit the level to move to the next level*
```
exit

```
<sub>Login to the next level to find how to beat it</sub>

```
 ssh bandit10@bandit.labs.overthewire.org -p 2220

```
```
==============================================
|         N E X T      L E V E L             | ===>
==============================================    
```
