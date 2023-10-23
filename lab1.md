# Lab 1 Ryan Chon
## CD
1. No argument


**input**
```
[user@sahara ~]$ cd lecture1
[user@sahara ~lecture1]$ cd 
[user@sahara ~]
```

* The working directory was lecture1
* When I did cd with no arguments it took me to the home directory. When cd has no arguments this is what is supposed to happen.
* It is not an error

2. With a path to a directory as an argument
```
[user@sahara ~]$ cd lecture1
[user@sahara ~lecture1]$  
```
* The working directory the command was run on was the home directory.
* This command when run with a path to a directory takes you into the drectory.
* There was no error.

3. File as argument
```
[user@sahara ~]$ cd lecture1
[user@sahara ~lecture1]$ ls 
Hello.class  Hello.java  messages  README
[user@sahara ~/lecture1]$ cd Hello.java
bash: cd: Hello.java: Not a directory
[user@sahara ~lecture1]$
```
* The working directory the command was run on was the lecture1.
* This instane of the commaand resulted in an error because Hello.java is not a directory.
* This is an error because a file is not a directory
---

## ls
1. No argument

```
[user@sahara ~]$ ls
lecture1
```
* the working directory of the command was the home directory
* This command lists the files and directorys inside of the dictory
* This is not an error
2. Directory Argument



```
[user@sahara ~]$ ls lecture1 
Hello.class  Hello.java  messages  README
```
* The working directory was the home directory
* When a path to a directory is an argument it will instead list the files of that directory instead of the original directory you are on.
* This is not an error
3. File Argument

```
[user@sahara ~/lecture1]$ ls Hello.java
Hello.java
[user@sahara ~/lecture1]$
```
* Working directory is in the lecture1 folder
* When used on a file, this command just repeats the name of the file.
* This is not an erro
---

## Cat
1. no argument



```
[user@sahara ~]$ cat

```
* Working Directory is the home directory
* When used on the home directory nothing happens and you must exit the command with ctrl+c
* This is an error because cat prints out a file and there is no target file
2. On directory


```
[user@sahara ~]$ cat lecture1
cat: lecture1: Is a directory
```
* Working Directory is the home directory
* When used on a directory it doesn't work and will instead just say that the argument is a directory. It makes sense since cat prints out a file not a directory.
* This is an error because cat prints out the contents of the file no directories
3. On a file as an argument


``` 
[user@sahara ~/lecture1]$ cat README
To use this program:

javac Hello.java
java Hello messages/en-us.txt
```
* Working Directory is Lecture1
* When used on a file, it prints out the contents of the file into the terminal.
* This is not an error