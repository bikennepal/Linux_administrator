# Linux_administrator

Linux bootcamp tutorial.
If you are using windows install Vm on your system you can go with minimal sio or dvd as well.
You can either install desktop distrubition or server distrubution.

connection over the network.
SSH
Windows- Putty
Mac-Terminal/ssh command line utility.
==============================================================
Linux fundamentals.

Linux Directory structure.
common directories:
/    "Root" the top of the file system hierarchy
/bin	Binaries and other executable programs.
/etc	System configuration files.
/home	user home directory
/opt	optional or third party software.
/tmp	Temporary space,typically cleared when rebooted.
/usr	User related programs
/var	Variable data, most notably log files
/boot	File need to boot the operating system.
/dev	Device files,typically controlled by operating system or the system administrator.
/export	Shared file systems.
/lib	System Libraries
/lib64  System Libraries,64bit.
/lost+found Used by the file system to store recovered files after a file system check has been performed
/media Used to mount removable medi like CD-Roms etc.
/mnt	Used to mount external file systems
/proc	Provides info about running processes
/Sbin	System adm binaries
/selinux	Used to display info abt SELinux.
/srv 	Contains data which is served by the server system.
/srv/www	Web Server files
/srv/ftp FTP files
/sys	Used to display and sometimes configure the devices known to the linux kernel
========================================
Application Directory Structures
/usr/local/crashplan/bin
/usr/local/crashplan/etc
/usr/local/crashplan/lib
/usr/local/crashplan/log
Many More.

====================================================
The Shell
The command line Interface to the Linux Operating System.It is the default interface to the kernel or Os.

======================================================================
Basic Linux command
The basic command that are used often are:
You know most of them.

============================================================
Getting Help at the command Line

Environment Variable:
All environment variable are in Upper-case letter.

PATH: Environment variable command.
Controls the command path search
contains a list of directories
==============================================
Working with directories
Something that is new to me: Environment variable to know the previous working state:echo $OLDPWD

To create more than one directory use -p as option.
example: mkdir -p dir1/dir2/dir3 

rmdir: remove empty directory. but to remove all the directory use:rm -rf command.

=========================================================================
Listing Files
If you run ls -f this command is used to check type of file.
tree command is used to dislay visual output.
exanple:tree
==========================================================================
File and directory permissions.
Symbolic permissions
Numeric /octal permissions
File versus directory permissions
changing permissions
working with groups
file creation mask.

Type of permissions
Read
write and 
execute
and permisson to each user is given as "u g o all" we can use "groups" command to see the user attached to which group.
to change permisson mod:chmod g+x etc.
go through umask once on youtube."basically it is a default file permission on linux"

================================================================
Finding files and directories
we can use find [path...] [expression]
we have another command "locate" which is not faster than find command.

========================================================================
viewings files and the nano editor
cat file   Display the content of the file
more file  Browse through a text file
less file  More features than more
head file  Output the beginning portion of the file
tail file  output the last line of the file
to see only limited line we can use tail -15 file-name. To see real time file use tail -f file

==============================================================================
Editing files with Emacs
Deleting, Copying, Movind and Renaming Files
rm file		Remove file
rm -r dir	Remove the directory and its contents recursively
rm -f file	Force removal of file.

copy
to copy files the command use is cp file1 file2 we are copying file1 to file2

rename a file or directory.
mv file1 as file2
mv to move frm one dir to other:mv source destination
sorting using sort command there are different ways to use sort command.
we can use sort command for various sorting.
gzip to compress and tar to make an archive file.

=====================================================================
Intermediate linux skills
wildcarts part one
a* means all that start with a and *a means all that ends with a.
A character class search pattern []
Name character classes are pre-defined
[[:alpha:]]
[[:alnum:]]
[[:digit:]]
[[:lower:]]
[[:space:]]
[[:upper:]]
perform some excercise on wild card

===============================================================
input output redirection
Three I/O types:SI stdin,SO stdin and SE 2
Redirection characters.






















