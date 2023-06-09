                     _                     _ _ _
                    | |__   __ _ _ __   __| (_) |_
                    | '_ \ / _` | '_ \ / _` | | __|
                    | |_) | (_| | | | | (_| | | |_
                    |_.__/ \__,_|_| |_|\__,_|_|\__|  



# LEVEL 6

## Level Goal:

-Find the password for the next level stored  *somewhere on the server* 
has all of the following properties:

owned by user bandit7
owned by group bandit6
33 bytes in size

## Level information:

| port |             host               |
|-----:|--------------------------------|
| 2220 |  bandit.labs.overthewire.org   |

| Level6|  Password                             |
|-------:|---------------------------------------|
| Bandit6| P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU    |

## Commands you may need to solve this level

```
ls
cd
cat
file
du
find
grep
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
find i -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null
``` 

`find` : Initiates the search command. 
`-type f`:Matches only regular files (excluding directories and other special file types). 
`-user bandit7`: Matches files owned by the user bandit7.
`-group bandit6`: Matches files owned by the group bandit6.
`-size 33c`: Matches files with a size of 33 bytes.
`2>/dev/null`: Redirects error messages to /dev/null to suppress any permission denied errors.

``` 
/var/lib/dpkg/info/bandit7.password
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
z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S

```

+ *Exit the level to move to the next level*
```
exit

```
<sub>Login to the next level to find how to beat it</sub>

```
 ssh bandit6@bandit.labs.overthewire.org -p 2220

```
```
==============================================
|         N E X T      L E V E L             | ===>
==============================================    
```
