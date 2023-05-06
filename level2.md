                     _                     _ _ _
                    | |__   __ _ _ __   __| (_) |_
                    | '_ \ / _` | '_ \ / _` | | __|
                    | |_) | (_| | | | | (_| | | |_
                    |_.__/ \__,_|_| |_|\__,_|_|\__|  



# LEVEL 2

## Level Goal:

-Find the password for the next level stored in the file *spaces in this filename* located in the home directory  , use it log into bandit3 .

## Level information:

| port |             host               |
|-----:|--------------------------------|
| 2220 |  bandit.labs.overthewire.org   |

| Level2 |  Password                             |
|-------:|---------------------------------------|
| Bandit2| NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL      |

## Commands you may need to solve this level

```
ls
cd
cat
file
du
find
```

## Step-by-step solutions:

+ *Log into the game* 
 Use this following code to enter the game=>
```
ssh bandit2@bandit.labs.overthewire.org -p 2220
```
<sub>We have to enter ssh following the host and the port which is 2220 to enter the level 2 with bandit2@host -p (port)</sub>

+ *Enter the password required* : 
```
NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL
```
<sub>We found it during the previous level</sub>

+Once we entered the game we will *search the file that contains the password* for the next level
```
ls
```
<sub>
  ls: List information about the FILEs (the current directory by default).
  ls will show the files
</sub>

``` 
cat 'spaces in this filename'
```
<sub>
  cat :  concatenate files and print on the standard output
  cat will show the content of the file : for this game , it will show the password for the next level
</sub>

``` 
rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi

```

+ *Exit the level to move to the next level*
```
exit

```
<sub>Login to the next level to find how to beat it</sub>
```
 ssh bandit3@bandit.labs.overthewire.org -p 2220

```
```
==============================================
|         N E X T      L E V E L             | ===>
==============================================    
```
