### Binaries 
This term refers to files that can be executed, similar to
executables in Windows. Binaries generally reside in the /usr/bin or
usr/sbin directory and include utilities such as ps, cat, ls, and ifconfig
(we’ll touch on all of four of these in this chapter) as well as applications such as the wireless hacking tool aircrack-ng and the intrusion
detection system (IDS) Snort.

### Case sensitivity 

Unlike Windows, the Linux filesystem is case sensitive. This means that Desktop is different from desktop, which is different
from DeskTop.

### Directory 
This is the same as a folder in Windows. A directory provides a way of organizing files, usually in a hierarchical manner
### Home 
Each user has their own /home directory, and this is generally
where files you create will be saved by default.
### Kali 
Kali Linux is a distribution of Linux specifically designed for
penetration testing
### root 
Like nearly every operating system, Linux has an administrator
or superuser account, designed for use by a trusted person who can do
nearly anything on the system. This would include such things as reconfiguring the system, adding users, and changing passwords. In Linux,
that account is called root. As a hacker or pentester, you will often use
the root account to give yourself control over the system. In fact, many
hacker tools require that you use the root account.
### Script 
This is a series of commands run in an interpretive environment that converts each line to source code. Many hacking tools are
simply scripts. Scripts can be run with the bash interpreter or any of
the other scripting language interpreters, such as Python, Perl, or Ruby.
Python is currently the most popular interpreter among hackers.

### Shell 
This is an environment and interpreter for running commands
in Linux. The most widely used shell is bash, which stands for Bourneagain shell, but other popular shells include the C shell and Z shell. I
will be using the bash shell exclusively in this book.

### Terminal 
This is a command line interface (CLI).

![image](https://github.com/Depth-monster/white_hat/assets/122405130/8c45b169-b1d6-4636-b0a1-a5eee2d9c0e1)

To get more information about the files and directories, such as their
permissions, owner, size, and when they were last modified, you can add
the -l switch after ls
### kali >ls -l

total 84

drw-r--r-- 1 root root 4096 Dec 5 11:15 bin

drw-r--r-- 2 root root 4096 Dec 5 11:15 boot

drw-r--r-- 3 root root 4096 Dec 9 13:10 dev

drw-r--r-- 18 root root 4096 Dec 9 13:43 etc

--snip--

drw-r--r-- 1 root root 4096 Dec 5 11:15 var

Some files in Linux are hidden and won’t be revealed by a simple ls or

ls -l command. To show hidden files, add a lowercase –a switch, like so:

### kali >ls -la
========
Nearly every command, application, or utility has a dedicated help file in
Linux that provides guidance for its use. For instance, if I needed help
using the best wireless cracking tool, aircrack-ng, I could simply type the
aircrack-ng command followed by the --help command:
### kali >aircrack-ng --help
### kali >nmap -h
Unfortunately, although many applications support all three options
(--help, -h, and -?), there’s no guarantee the application you’re using will.
So if one option doesn’t work, try another
