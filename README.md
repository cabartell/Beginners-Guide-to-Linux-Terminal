# Beginners-Guide-to-Linux-Terminal

The Linux terminal is a text interface to your computer. Often referred to as the shell, commandline, console, prompt or various other names. As a beginner, it may seem complex and confusing to use but you get used to it quite fast. 
## Location & the cd command
When typing in commands, remember that commands are usually case sensitive so typing a command like `pwd` in all caps (`PWD`) could give you a completely different outcome and in some cases, mess up some things. So always double-check :)

Speaking of the `pwd` command, this command is short for "Print Working Directory" and will tell you which folder you're in! It's useful if you're ever trying to get into a certain folder and are unsure! One important concept to understand is that the terminal assumes the folder you are in as default location in which any file operations will take place. This is its working directory. If you try to create new files or directories, view existing files, or delete them, the terminal will assume you’re looking for them in the current working directory unless you specify otherwise. So it’s important to know what directory you are in at any given time, after all,deleting files from the wrong directory could be disastrous.    

To go to a different directory, you can use the `cd` command. This is short for "change directory". The base directory is `/`. If you're used to windows, this is the equivalent of, for example, `C:` for the C drive. Unix-based systems don't split up the drives and just have one single file system consisting of drives mounted/attached to whatever location in the file system suits it. Everything branching out from the `/` directory.

### Superuser
Beware that although the `/` directory is sometimes referred to as the root directory, the word "root" has another meaning. root is also the name that has been used for the superuser since the early days of Unix. The superuser, as the name suggests, has more powers than a normal user and can easily wreak havoc with a wrong command.

## Folders and files
To learn about files, we'll first need to create some to play around with. Let's start by making a new folder, also called a directory, to store our files in with `mkdir <foldername>`    
For example:    
```
mkdir test
```
this command only works if you are inside the folder you want to make your new folder in. If you want to make a folder in a different directory than the one you are in, you will need to provide the path    
For example:    
```
mkdir /tmp/test
```
The command will try to find the 'tmp' directory and create the 'test' folder in it.    
In case you hadn't guess it already, 'mkdir' is short for "make directory" ;)    
To go into your newly created folder, you use the `cd` command, its syntax is similar to the mkdir command you just used    
```
cd test
```
or
```
cd /tmp/test
```
to check with folder you're currently in, use the `pwd`    
Now we can create some subfolders    
```
mkdir test1 test2 test3
```
this will create 3 folders in the dirctory you are currently in.    
You can check what's in you current directory with the `ls` command    
