                     _                     _ _ _
                    | |__   __ _ _ __   __| (_) |_
                    | '_ \ / _` | '_ \ / _` | | __|
                    | |_) | (_| | | | | (_| | | |_
                    |_.__/ \__,_|_| |_|\__,_|_|\__|  



# LEVEL 17

## Level Goal:

There are 2 files in the homedirectory: passwords.old and passwords.new. 
The password for the next level is in passwords.new and is the only line that has been changed between passwords.old and passwords.new


## Level information:

| port |             host               |
|-----:|--------------------------------|
| 2220 |  bandit.labs.overthewire.org   |

| Level17  |    Password                           |
|-------:  |---------------------------------------|
| Bandit17 |    cluFn7wTiGryunymYOu4RcffSxQluehd   |

## Commands you may need to solve this level

```
cat, grep, ls, diff
```

## Step-by-step solutions:
+Login : `ssh -i sshkey17.private 
bandit17@bandit.labs.overthewire.org -p 2220`
SSH : (Private SSH key from the previous level)

+ We will sort the password.old and password.new of the file based on the level 9 .



```
 sort passwords.old passwords.new | uniq -u
 ```
 ```
kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd
w0Yfolrc5bwjS4qw5mq1nnQi6mF03bii
cat passwords.new | grep w0Yfolrc5bwjS4qw5mq1nnQi6mF03bii
cat passwords.new | grep kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd
kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd
```






==============================================
|         N E X T      L E V E L             | ===>
==============================================    
```
