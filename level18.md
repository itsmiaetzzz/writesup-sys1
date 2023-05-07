                     _                     _ _ _
                    | |__   __ _ _ __   __| (_) |_
                    | '_ \ / _` | '_ \ / _` | | __|
                    | |_) | (_| | | | | (_| | | |_
                    |_.__/ \__,_|_| |_|\__,_|_|\__|  



# LEVEL 17

## Level Goal:

The password for the next level is stored in a file readme in the homedirectory. 
Unfortunately, someone has modified .bashrc to log you out when you log in with SSH.


## Level information:

| port |             host               |
|-----:|--------------------------------|
| 2220 |  bandit.labs.overthewire.org   |

| Level18  |    Password                           |
|-------:  |---------------------------------------|
| Bandit18 |    kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd   |

## Commands you may need to solve this level

```
ssh, ls, cat
```

## Step-by-step solutions:

+Login :

 ```
 ssh bandit18@bandit.labs.overthewire.org -p 2220 ls
 
 ```
<sub>Instead of logging into the machine with SSH,
  we execute a command through SSH instead. 
  First, we use `ls` to make sure the readme file is in the folder then we can use `cat` to read it.</sub>
  

```
bandit18@bandit.labs.overthewire.org's password: 
readme

$ ssh bandit18@bandit.labs.overthewire.org -p 2220 cat readme 
This is a OverTheWire game server. More information on http://www.overthewire.org/wargames

bandit18@bandit.labs.overthewire.org's password: 
IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x
 ```






```
==============================================
|         N E X T      L E V E L             | ===>
==============================================    
```
