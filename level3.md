                     _                     _ _ _
                    | |__   __ _ _ __   __| (_) |_
                    | '_ \ / _` | '_ \ / _` | | __|
                    | |_) | (_| | | | | (_| | | |_
                    |_.__/ \__,_|_| |_|\__,_|_|\__|  



# LEVEL 3

## Level Goal:

-Find the password for the next level stored in a *hidden file* located in in the *inhere* directory.

## Level information:

| port |             host               |
|-----:|--------------------------------|
| 2220 |  bandit.labs.overthewire.org   |

| Level3 |  Password                             |
|-------:|---------------------------------------|
| Bandit3| aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG      |

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
aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG
```
<sub>We found it during the previous level</sub>

+Once we entered the game we will *search the file that contains the password* for the next level that is hidden .


<sub>
 Here the file is in the *inhere* directory so, we will change the directory:
</sub>

```
cd inhere

```

<sub>
After that , we will show the hidden file 
</sub>

```
ls -a

```

<sub>

  ls -a : lists all files and directories in the current directory, including hidden files. 
  
</sub>

``` 
.  ..  .hidden
```

``` 
cat .hidden
```
<sub>
  cat :  concatenate files and print on the standard output
  cat will show the content of the file : for this game , it will show the password for the next level
</sub>


``` 
2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe

```

+ *Exit the level to move to the next level*
```
exit

```
<sub>Login to the next level to find how to beat it</sub>

```
 ssh bandit4@bandit.labs.overthewire.org -p 2220

```
```
==============================================
|         N E X T      L E V E L             | ===>
==============================================    
```
