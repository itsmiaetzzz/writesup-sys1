                     _                     _ _ _
                    | |__   __ _ _ __   __| (_) |_
                    | '_ \ / _` | '_ \ / _` | | __|
                    | |_) | (_| | | | | (_| | | |_
                    |_.__/ \__,_|_| |_|\__,_|_|\__|  



# LEVEL 8

## Level Goal:


The password for the next level is stored in the file *data.txt* and is the *only line of text that occurs only once*.

## Level information:

| port |             host               |
|-----:|--------------------------------|
| 2220 |  bandit.labs.overthewire.org   |

| Level8 |    Password                           |
|-------:|---------------------------------------|
| Bandit8|   TESKZC0XvTetK0S9xNwm25STk5iWrBvP    |

## Commands you may need to solve this level

```
uniq , cat , ls 
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
 TESKZC0XvTetK0S9xNwm25STk5iWrBvP
```
<sub>We found it during the previous level</sub>

+Once we entered the game we will *search the file that contains the password* for the next level that is somewhere on the server .


We will use the find to write this statement



``` 
 grep -v -F -x -f <(sort data.txt | uniq -d) data.txt

```
<sub>
 `grep`: searches for lines
`-v` :inverts the match, so it shows lines that do not match.
`-F` :treats the patterns as fixed strings, not regular expressions.
`-x`:matches whole lines.
`-f <(sort data.txt | uniq -d)`: specifies the file to read the patterns from, which is the sorted duplicate lines .
`data.txt` is the file to search in.
==========
`sort data.txt | uniq -d`:sorts the lines in the "data.txt" file and extracts only the duplicate line.
 `uniq -d`  :  specifies that only duplicate lines should be shown
`<(...)` is a convenient syntax that allows you to manipulate the output of a command as if it were stored in a file, without the need to create an actual file on the file system.
</sub>
 
```
EN632PlfYiZbn3PhVK3XOGSlNInNE00t
```
+ *Exit the level to move to the next level*
```
exit

```
<sub>Login to the next level to find how to beat it</sub>

```
 ssh bandit9@bandit.labs.overthewire.org -p 2220

```
```
==============================================
|         N E X T      L E V E L             | ===>
==============================================    
```
