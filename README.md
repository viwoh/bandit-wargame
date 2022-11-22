# Bandit Wargame
## OverTheWire's Bandit challenges to learn and practice security concepts.
<p align="center"> <img src="https://media.tenor.com/1G7KLUiquh0AAAAi/typing-fast.gif"> 

<p align="center">================LVL 0 BANDIT================

Commands to establish connection via SSH with user bandit0 on the port 2220 (the default port is 22)
ssh bandit0@bandit.labs.overthewire.org -p 2220

After listing the files in the folder was found a readme file, containing the following text: NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL

Command "ls" was used to list the content in the directory.


<p align="center">================LVL 1 BANDIT================

Commands to establish connection via SSH with user bandit1 on the port 2220 (the default port is 22)

ssh bandit1@bandit.labs.overthewire.org -p 2220

Command "ls" was used and it was found a file with a dashed name "-". So it was necessary to use the command "cat ./-" to read it. The following text was found: rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi


<p align="center"> ================LVL 2 BANDIT================

Commands to establish connection via SSH with user bandit2 on the port 2220 (the default port is 22)

ssh bandit2@bandit.labs.overthewire.org -p 2220

Command "ls" was used and it was found a file named "spaces in this filename". So it was necessary to read it using the following method:

cat spaces\ in\ this\ filename

Then it was found the password to the next level: aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG


<p align="center">================LVL 3 BANDIT================

Commands to establish connection via SSH with bandit3 on the port 2220 (the default port is 22)

ssh bandit3@bandit.labs.overthewire.org -p 2220

Command ls was used and it was found a directory named "inhere", after entering it, it was necessary to use the command "ls -a" to list everything, because the file - named hidden - was hidden.

Then it was found the password to the next level:
2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe


<p align="center">================LVL 4 BANDIT================

Commands to establish connection via SSH with bandit4 on the port 2220 (the default port is 22)

ssh bandit4@bandit.labs.overthewire.org -p 2220

Command "ls" was used and it was found a directory named "inhere". To enter the directory, it was used the command "cd" and then "ls" to list the files, resulting on the following:
-file00  -file02  -file04  -file06  -file08                                        -file01  -file03  -file05  -file07  -file09

It was necessary to use to use the command "cat ./-" to read it, since the filename iniciated with a dash it was being considered as a flag to the command. When opened the -file07 ("cat ./-file07"), it was found the password:
lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR


<p align="center">================LVL 5 BANDIT================

Commands to establish connection via SSH with bandit5 on the port 2220 (the default port is 22)

ssh bandit5@bandit.labs.overthewire.org -p 2220

Entering the "inhere" directory and using the command "find . -size 1033c" to search for all files with the size of 1033 bytes, the only one found was the hidden file ".file2" in the "maybehere07" directory. Its content was read by using "cat ./.file2" and returned the password:
P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU


