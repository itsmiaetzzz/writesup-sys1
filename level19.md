                     _                     _ _ _
                    | |__   __ _ _ __   __| (_) |_
                    | '_ \ / _` | '_ \ / _` | | __|
                    | |_) | (_| | | | | (_| | | |_
                    |_.__/ \__,_|_| |_|\__,_|_|\__|  



# LEVEL 19

## Level Goal:
To gain access to the next level, you should use the setuid binary in the homedirectory. Execute it without arguments to find out how to use it. The password for this level can be found in the usual place (/etc/bandit_pass), after you have used the setuid binary.


## Level information:

| port |             host               |
|-----:|--------------------------------|
| 2220 |  bandit.labs.overthewire.org   |

| Level19  |    Password                           |
|-------:  |---------------------------------------|
| Bandit19 |    IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x   |

## Commands you may need to solve this level

```
setuid
```

## Step-by-step solutions:

+Lists of the file :

```
ls -a
```
```
.  ..  .bash_logout  .bashrc  .profile  bandit20-do
```
 

+Running a command as another user  
```
 ./bandit20-do mia

```
```
 ./bandit20-do cat /etc/bandit_pass/bandit20

```
```
GbKksEFF4yrVs6il55v6gwY5aVje5f0j
```






```
==============================================
|         N E X T      L E V E L             | ===>
==============================================    
```
