                     _                     _ _ _
                    | |__   __ _ _ __   __| (_) |_
                    | '_ \ / _` | '_ \ / _` | | __|
                    | |_) | (_| | | | | (_| | | |_
                    |_.__/ \__,_|_| |_|\__,_|_|\__|  



# LEVEL 12

## Level Goal:

The password for the next level is stored in the file *data.txt*, which is a* hexdump of a file that has been repeatedly compressed*.
For this level it may be useful to *create a directory under /tmp *in which you can work using *mkdir*. For example: mkdir /tmp/myname123.
Then copy the *datafile using cp*, and *rename it using mv* (read the manpages!)



## Level information:

| port |             host               |
|-----:|--------------------------------|
| 2220 |  bandit.labs.overthewire.org   |

| Level12   |    Password                          |
|-------:  |---------------------------------------|
| Bandit12 |   JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv    |

## Commands you may need to solve this level

```
cat , tr 
```

## Step-by-step solutions:

+ *Log into the game* 
 Use this following code to enter the game=>
```
ssh bandit12@bandit.labs.overthewire.org -p 2220
```
<sub>We have to enter ssh following the host and the port which is 2220 to enter the level  with banditN°level@host -p (port)</sub>

+ *Enter the password required* : 
```
JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv
```
<sub>We found it during the previous level</sub>

+Once we entered the game we will *search the file that contains the password* for the next level. 
We will use the commands  `cat` and `echo tr ` to write this statement



``` 
 cat data.txt 
```


 `cat`: show the the content of the file
`data.txt` : is the file to search in.
 `tr`command-line utility for translating or deleting characters

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
