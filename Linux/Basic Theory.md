### **1.1 Filesystem Hierarchy**


Linux follows a strict structure:

- / – root of the entire filesystem
    
- /home/username – your personal space
    
- Everything is a file (even devices, configs)
    


macOS is close but includes /System, /Library, /Users etc. Same concepts apply.

  
### **1.2 Navigation**

- pwd — print working directory
    
- cd — change directory
    
- ls — list directory contents
    
- ls -l — long listing format
    
- ls -a — show hidden files
    
- .. — parent directory
    
- . — current directory (it tells the system “don’t look elsewhere; look **right here**”)
    
- ~ — home directory


> [!NOTE] Title
> **nano** - is a terminal text editor
> **#!/bin/bash** - this is a first line of a script file it tells the OS to use this file as a programm to run a script

* **$PATH** - it is an env variable. Or it is just a search list.

* **[[find]]** - a command is used to find for files or directories. Contains given path where to search and given condition (like name, or file type, etc.)
* **[[grep]]** - a command stands for searching for informations inside files. Also can have different variations of usage. 
#### **Redirection**

- > — send output to a file (overwrite)
    
- >> — send output to a file (append)
    
- < — use file content as input to a command
    

#### **Pipes**

- | — take output of one command and use it as input for the next

* **[[Processes]]** - they are the same as we use диспетчер задач. Key command will add to the link. 
  Commands - ps, bg, top, fg


> [!REMEMBER] REMEMBER
> && - it is simple AND operator like in programming or SQL
> | - it takes output from the first command and uses it in second command
> 
