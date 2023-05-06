                     _                     _ _ _
                    | |__   __ _ _ __   __| (_) |_
                    | '_ \ / _` | '_ \ / _` | | __|
                    | |_) | (_| | | | | (_| | | |_
                    |_.__/ \__,_|_| |_|\__,_|_|\__|  



# LEVEL 5

## Level Goal:

-Find the password for the next level stored in a *stored file* located in the *inhere* directory with properties : 
                        human-readable /
                        1033 bytes in size /
                        not executable.

## Level information:

| port |             host               |
|-----:|--------------------------------|
| 2220 |  bandit.labs.overthewire.org   |

| Level5 |  Password                             |
|-------:|---------------------------------------|
| Bandit5| lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR     |

## Commands you may need to solve this level

```
find
cat

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

+Once we entered the game we will *stored file* located in the *inhere* directory with properties : human-readable /1033 bytes in size /not executable. that contains the password* for the next level 


<sub>
We will use the find to write this statement 
</sub>

```
find inhere -type f -readable ! -executable -size 1033c

```

<sub>
`find` : Initiates the search command.
 `inhere`: Specifies the starting directory for the search.
`-type f`: Matches only regular files (excluding directories and other special file types).
`-readable`: Matches files that are readable.
</sub>

```
inhere/maybehere07/.file2

```
<sub>
It shows us the file that correspond with the properties defined.
</sub>

+We will enter this file and show the password.

```
cat .file2

```
<sub>
cat : Displays the contents of a file.
</sub>

``` 
P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU

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
