# Shell are executables files
The default shell on most Linux system is bash, it is an ordinary program, with an executable file located in /bin, together with other familiar command like cat, ls or grep. 

You can find all the valid shell on you system in the file /etc/shells :

$cat /etc/shells

# /etc/shells: valid login shells
/bin/sh
/bin/dash
/bin/bash
/bin/rbash

To see which shell you are running, check the variable SHELL:
$echo $SHELL
/bin/bash

In theory a Linux system can treat any program as a valid login shell, if it is listed in the file /etc/shells.
Using superuser privileges, your own shell can be installed. In this example I'm creating a simple damn shell that reads any command and reply.
This custom shell is intentionally silly, but it donstrates that also other program can be a legitimate shell.

