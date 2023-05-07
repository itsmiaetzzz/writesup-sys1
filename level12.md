                     _                     _ _ _
                    | |__   __ _ _ __   __| (_) |_
                    | '_ \ / _` | '_ \ / _` | | __|
                    | |_) | (_| | | | | (_| | | |_
                    |_.__/ \__,_|_| |_|\__,_|_|\__|  



# LEVEL 12

## Level Goal:

The password for the next level is stored in the file *data.txt*, which is a* hexdump of a file that has been repeatedly compressed*.
For this level it may be useful to *create a directory under /tmp *in which you can work using *mkdir*. For example: mkdir /tmp/myname123.
Then copy the *datafile using cp*, and *rename it using mv* (read the manpages!)



## Level information:

| port |             host               |
|-----:|--------------------------------|
| 2220 |  bandit.labs.overthewire.org   |

| Level12   |    Password                          |
|-------:  |---------------------------------------|
| Bandit12 |   JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv    |

## Commands you may need to solve this level

```
mv: rename a file
cp : copy data file 
mkdir : create a directory 

```

## Step-by-step solutions:

+ *Log into the game* 
 Use this following code to enter the game=>
```
ssh bandit12@bandit.labs.overthewire.org -p 2220
```
<sub>We have to enter ssh following the host and the port which is 2220 to enter the level  with banditN°level@host -p (port)</sub>

+ *Enter the password required* : 
```
JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv
```
<sub>We found it during the previous level</sub>

+Once we entered the game we will *search the file that contains the password* for the next level. 
We will use the commands  `` and `echo tr ` to write this statement


=> Show all the files 
``` 
 ls -a

```
```
.  ..  .bash_logout  .bashrc  data.txt  .profile
```

=> Create a directory with mkdir 
```
mkdir /tmp/mialtina
``` 

=>  reverse the hexadecimal dump stored in the file data.txt and generate the corresponding binary output
```
xxd -r data.txt > /tmp/mialitina/file.bin

```
=> change directory 
```
cd /tmp/mialitina
```

```
ls -a
```
```
.  ..  file.bin
```
=>  `file` + file_name : analyzes the contents of the file.bin file and provides information about its type.
```
file file.bin
```
```
file.bin: gzip compressed data, was "data2.bin", last modified: Sun Apr 23 18:04:23 2023, max compression, from Unix, original size modulo 2^32 581
```
=> `zcat` , `bzcat`:decompresses the contents of file.bin and outputs the uncompressed data to the standard output
    `tar xO`:used to extract a single file from a tar archive and write its contents to the standard output (stdout) instead of creating a file on disk
```
zcat file.bin | file -
```
```
/dev/stdin: bzip2 compressed data, block size = 900k
```

```
zcat file.bin |bzcat| file -
```
```
/dev/stdin: gzip compressed data, was "data4.bin", last modified
: Sun Apr 23 18:04:23 2023, max compression, from Unix
```

```
zcat file.bin | bzcat | zcat | file -
```

```
/dev/stdin: POSIX tar archive (GNU)
```


```
 zcat file.bin | bzcat | zcat|tar xO |tar xO |file -
```
```
/dev/stdin: bzip2 compressed data, block size = 900k
```

```
zcat file.bin | bzcat | zcat|tar xO |tar xO |bzcat   |tar xO|file -t file.bin | bzcat | zcat|tar xO |
```
```
/dev/stdin: gzip compressed data, was "data9.bin", last modified: Sun Apr 23 18:04:23 2023, max compression, from Unix
```


```
 zcat file.bin | bzcat | zcat | tar xO | tar xO | bzcat | tar xO | zcat | file -
```
```
/dev/stdin: ASCII text
```

```
 zcat file.bin | bzcat | zcat | tar xO | tar xO | bzcat | tar xO | zcat
```
```
The password is wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw
```


```
+ *Exit the level to move to the next level*
```
exit

```
<sub>Login to the next level to find how to beat it</sub>

```
 ssh bandit12@bandit.labs.overthewire.org -p 2220

```
```
==============================================
|         N E X T      L E V E L             | ===>
==============================================    
```
