                     _                     _ _ _
                    | |__   __ _ _ __   __| (_) |_
                    | '_ \ / _` | '_ \ / _` | | __|
                    | |_) | (_| | | | | (_| | | |_
                    |_.__/ \__,_|_| |_|\__,_|_|\__|  



# LEVEL 11

## Level Goal:

The password for the next level is stored in the file *data.txt*, where *all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 position*



## Level information:

| port |             host               |
|-----:|--------------------------------|
| 2220 |  bandit.labs.overthewire.org   |

| Level9   |    Password                           |
|-------:  |---------------------------------------|
| Bandit11 |    6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM   |

## Commands you may need to solve this level

```
cat , tr 
```

## Step-by-step solutions:

+ *Log into the game* 
 Use this following code to enter the game=>
```
ssh bandit11@bandit.labs.overthewire.org -p 2220
```
<sub>We have to enter ssh following the host and the port which is 2220 to enter the level 10 with bandit10@host -p (port)</sub>

+ *Enter the password required* : 
```
6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM
```
<sub>We found it during the previous level</sub>

+Once we entered the game we will *search the file that contains the password* for the next level. 
We will use the commands  `cat` and `echo tr ` to write this statement



``` 
 cat data.txt 
```

<sub>
 `cat`: show the the content of the file
`data.txt`: is the file to search in.
 `tr`command-line utility for translating or deleting characters
</sub>
```
Gur cnffjbeq vf WIAOOSFzMjXXBC0KoSKBbJ8puQm5lIEi
``` 
<sub>Now , we will find the password and apply the ROT13 </sub>

```
 echo " Gur cnffjbeq vf WIAOOSFzMjXXBC0KoSKBbJ8puQm5lIEi" | tr 'A-Za-z' 'N-ZA-Mn-za-m'
```
<sub>  
  'A-Za-z' 'N-ZA-Mn-za-m' : rotate 13 

</sub>

```
The password is JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv
```
+ *Exit the level to move to the next level*
```
exit

```
<sub>Login to the next level to find how to beat it</sub>

```
 ssh bandit12@bandit.labs.overthewire.org -p 2220

```
```
==============================================
|         N E X T      L E V E L             | ===>
==============================================    
```
