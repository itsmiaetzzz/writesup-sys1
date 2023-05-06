                     _                     _ _ _
                    | |__   __ _ _ __   __| (_) |_
                    | '_ \ / _` | '_ \ / _` | | __|
                    | |_) | (_| | | | | (_| | | |_
                    |_.__/ \__,_|_| |_|\__,_|_|\__|  



# LEVEL 5

## Level Goal:

-Find the password for the next level stored in a *stored file* located in the *inhere* directory with properties : 
                        human-readable
                        1033 bytes in size
                        not executable

## Level information:

| port |             host               |
|-----:|--------------------------------|
| 2220 |  bandit.labs.overthewire.org   |

| Level5 |  Password                             |
|-------:|---------------------------------------|
| Bandit5| lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR     |

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
ssh bandit5@bandit.labs.overthewire.org -p 2220
```
<sub>We have to enter ssh following the host and the port which is 2220 to enter the level 2 with bandit2@host -p (port)</sub>

+ *Enter the password required* : 
```
lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR
```

<sub>We found it during the previous level</sub>

+Once we entered the game we will *search the only human-readable file that contains the password* for the next level in the *inhere* directory .


<sub>
 Here the file is in the *inhere* directory so, we will change the directory:
</sub>

```
cd inhere

```

<sub>
After that , we will show the only human-readable file
</sub>

```
ls -h

```

<sub>

  ls -h : is used to display the file size in a human readable way
  
</sub>

``` 
-file00  -file02  -file04  -file06  -file08
-file01  -file03  -file05  -file07  -file09

```
<sub>

  `file ./*`: provide information about each file in the directory, including the file type
  
</sub>

``` 
./-file00: data
./-file01: data
./-file02: data
./-file03: data
./-file04: data
./-file05: data
./-file06: data
./-file07: ASCII text
./-file08: data
./-file09: Non-ISO extended-ASCII text, with no line terminators

```


```
cat  ./-file07

```

<sub>
   ./-file07 : this is the only human readable file ASCII text
  cat will show the content of the file : for this game , it will show the password for the next level
</sub>


``` 
lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR

```

+ *Exit the level to move to the next level*
```
exit

```
<sub>Login to the next level to find how to beat it</sub>

```
 ssh bandit5@bandit.labs.overthewire.org -p 2220

```
```
==============================================
|         N E X T      L E V E L             | ===>
==============================================    
```
