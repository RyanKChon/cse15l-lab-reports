# Lab 1 Ryan Chon
## CD
1. No argument

The working directory was lecture1

**input**
```
[user@sahara ~]$ cd lecture1
[user@sahara ~lecture1]$ cd 
[user@sahara ~]
```
When I did cd with no arguments it took me to the home directory. When cd has no arguments this is what is supposed to happen.

It is not an error

2. With a path to a directory as an argument
```
[user@sahara ~]$ cd lecture1
[user@sahara ~lecture1]$  
```
The working directory the command was run on was the home directory.

This command when run with a path to a directory takes you into the directory. There was no error.

3. File as argument
```
[user@sahara ~]$ cd lecture1
[user@sahara ~lecture1]$ ls 
Hello.class  Hello.java  messages  README
[user@sahara ~/lecture1]$ cd Hello.java
bash: cd: Hello.java: Not a directory
[user@sahara ~lecture1]$
```
The working directory the command was run on was the home directory.

This instane of the commaand resulted in an error because Hello.java is not a directory.

---

## ls
1. No argument

```
[user@sahara ~]$ ls
lecture1
```
the working directory of the command was the home directory

This command lists the files and directorys inside of the dictory

2. Directory Argument

The working directory was the home file

```
[user@sahara ~]$ ls lecture1 
Hello.class  Hello.java  messages  README
```

When a path to a directory is an argument it will instead list the files of that directory instead of the original directory you are on.

3. File Argument

Working directory is in the lecture1 folder

```
[user@sahara ~/lecture1]$ ls Hello.java
Hello.java
[user@sahara ~/lecture1]$
```
When used on a file, this command just repeats the name of the file.

---

## Cat
1. no argument

Working Directory is the home directory

```
[user@sahara ~]$ cat

```

When used on the home directory nothing happens and you must exit the command with ctrl+c

2. On directory
Working Directory is the home directory

```
[user@sahara ~]$ cat lecture1
cat: lecture1: Is a directory
```
When used on a directory it doesn't work and will instead just say that the argument is a directory. It makes sense since cat prints out a file not a directory.

3. On a file as an argument

Working Directory is Lecture1
``` 
[user@sahara ~/lecture1]$ cat README
To use this program:

javac Hello.java
java Hello messages/en-us.txt
```
When used on a file, it prints out the contents of the file into the terminal.