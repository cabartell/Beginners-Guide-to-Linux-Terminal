# Beginners-Guide-to-Linux-Terminal

The Linux terminal is a text interface to your computer. Often referred to as the shell, commandline, console, prompt or various other names. As a beginner, it may seem complex and confusing to use but you get used to it quite fast.    

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
