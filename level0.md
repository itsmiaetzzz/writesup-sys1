                     _                     _ _ _
                    | |__   __ _ _ __   __| (_) |_
                    | '_ \ / _` | '_ \ / _` | | __|
                    | |_) | (_| | | | | (_| | | |_
                    |_.__/ \__,_|_| |_|\__,_|_|\__|  



# LEVEL 0

## Level Goal:

-log into the game using SSH , go to the Level 1 page to find out how to beat Level 1.
- search the *README* file which inculdes the password 

## Level information:

| port |             host               |
|-----:|--------------------------------|
| 2220 |  bandit.labs.overthewire.org   |

| Username |  Password      |
|---------:|----------------|
| bandit0  |  bandit0       |

## Commands you may need to solve this level

```
ssh
```

## Step-by-step solution:

+ *Log into the game* 
Use this following code to enter the game=>
```
ssh bandit0@bandit.labs.overthewire.org -p 2220
```
<sub>We have to enter ssh following the host and the port which is 2220 to enter the level 0 with bandit0@host -p (port)</sub>

+ *Enter the password required* : 
```
bandit0
```

+ *Search the file* : 
```
 ls 
```
<sub>ls : list the files and directories in the current directory </sub>
```
readme 
```
+ *Display the content of the file* : 
```
cat readme

```

```

NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL

```

Once we entered the game we will go to the level 1 by exit .
+ *Exit the level0 to move to the level 1 *
```
Exit

```
<sub>Login to the next level to find how to beat it</sub>
```
 ssh bandit1@bandit.labs.overthewire.org -p 2220

```
```
==============================================
|         N E X T      L E V E L             | ===>
==============================================    
```
