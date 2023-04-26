# SMART GRABS BELOW
### HOW TO CHANGE YOUR NAME FROM THE COMMAND LINE TO GITHUB
- git config user.name "New Name"
### SOME WORKABLE COMMANDS NEEDED FOR PERFORMANCE IN SHELL
- awk # pattern scanning and processing language
- basename # strip directory and suffix from filenames
- bg # resumes suspended jobs without bringing them to the foreground
- cat # print files
- cd # change the shell working directory.
- chmod # change file mode
- chown # change file owner and group
- crontab # maintain crontab files
- curl # transfer a URL
- cut # remove sections from each line of files
- date # display or set date and time
- dig # DNS lookup utility
- df # report file system disk space usage
- diff # compare files line by line
- du # estimate file space usage
- echo # display a line of text
- find # search for files in a directory hierarchy
- fg # resumes suspended jobs and bring them to the foreground
- grep # print lines matching a pattern
- kill # send a signal to a process
- less # read file with pagination
- ln # create links
- ls # list directory contents
- lsb_release # print distribution-specific information
- lsof # list open files
- mkdir # create
- mv # move files
- nc # arbitrary TCP and UDP connections and listens
- netstat # print network connections, routing tables, interface statistics...
- nice # execute a utility with an altered scheduling priority
- nproc # print the number of processing units available
- passwd # change user password
- pgrep # look up processes based on name and other attributes
- pkill # send signal to processes based on name and other attributes
- printenv # print all or part of environment
- pwd # print name of current/working directory
- top # display Linux processes
- tr # translate or delete characters
- ps # report a snapshot of the current processes
- rm # remove files or directories
- rmdir # remove directories
- rsync # remote file copy
- scp # secure copy (remote file copy program)
- sed # stream editor for filtering and transforming text
- sleep # suspend execution for an interval of time
- sort # sort lines of text file
- ssh # OpenSSH SSH client (remote login program)
- ssh-keygen # SSH key generation, management and conversion
- su # substitute user identity
- sudo # execute a command as another user
- tail # output the last part of files
- tar # manipulate archives files
- tr # translate or delete characters
- uname # Print operating system name
- uniq # report or omit repeated lines
- uptime # show how long system has been running
- w # Show who is logged on and what they are doing
- whereis # locate the binary, source, and manual page files for a command
- which # locate a command
- wc # print newline, word, and byte counts for each file
- xargs # build and execute command lines from standard input
- | # redirect standard output to another command
- ~> # redirect standard output
- < # redirect standard input
- & # send process to background
### IMPORTANT SHORCUTS
 - CTRL+A # go to beginning of line
 - CTRL+B # moves backward one character
 - CTRL+C # stops the current command
 - CTRL+D # deletes one character backward or logs out of current session
 - CTRL+E # go to end of line
 - CTRL+F # moves forward one character
 - CTRL+G # aborts the current editing command and ring the terminal bell
 - CTRL+K # deletes (kill) forward to end of line
 - CTRL+L # clears screen and redisplay the line
 - CTRL+N # next line in command history
 - CTRL+R # searches in your command history
 - CTRL+T # transposes two characters
 - CTRL+U # kills backward to the beginning of line
 - CTRL+W # kills the word behind the cursor
 - CTRL+Y # retrieves last deleted string
 - CTRL+Z # stops the current command, resume with fg in the foreground or bg in the background
# SHELL TUTORIALS PROPER
##### WHAT IS SHELL
-> Shell takes commands from the keyboard and give them to the operating system to perform. Shells are known as command line interface. CLI's

- For Study and clarity sake we will be learning with the unix system (Linux). In the shell a program called BASH (Bourne Again SHell) is used in written commands to the computer system. Theere are other programs called KSH, TCSH & ZSH these are also on the availbale on the Linux systems. It is important to note that the BASH is the enhanced version of the former version of the unix shell program SH.

##### A TERMINAL
-> This is a program that opens a window and lets you interact with the shell. There are many terminals though like the gnome-terminal, konsole, xterm, rxvt, kvt, nxterm, and eterm they are all included in some Linux distributions.

-> In shell there is availablity for command history. this was inserted to help users not to repeat the process of typing the commands over and over again. It is expedient to know that when you handle this command history, once the terminal closes the history is lost.

#### NAVIGATION
-> There are 3 basic commands used in navigating the linux environs
- CD: which means Change Directory
- PWD: which means Print Working Dir (note that DIR is same thing as Directory)
- LS: which means List files and Directories.

#### FILE SYSTEM ORGANIZATION
* The files of a linusx system is arranged in what is called Hierarchical Directory Structure. They are organised like a tree.
* Linux system does no use drive letters to indicate location of directories like in windows.
* It is expidient to note that "One important difference between Windows and Unix-like operating systems such as Linux is that Linux does not employ the concept of drive letters. While Windows drive letters split the file system into a series of different trees (one for each device), Linux always has a single tree. Different storage devices may be different branches of the tree, but there is always just a single tree".

