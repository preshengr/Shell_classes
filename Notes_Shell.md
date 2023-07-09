# SMART GRABS BELOW
### HOW TO CHANGE YOUR NAME FROM THE COMMAND LINE TO GITHUB
```
git config user.name "New Name"
```
### SOME WORKABLE COMMANDS NEEDED FOR PERFORMANCE IN SHELL
| COMMAND | DESCRIPTION |
| ------- | ----------- |
|awk|pattern scanning and processing language |
|basename|strip directory and suffix from filenames|
|bg |resumes suspended jobs without bringing them to the foreground|
|cat|print files|
|cd|change the shell working directory.|
|chmod|change file mode|
|chown|change file owner and group|
|crontab|maintain crontab files|
|curl|transfer a URL|
|cut|remove sections from each line of files|
|date|display or set date and time|
|dig|DNS lookup utility|
|df|report file system disk space usage|
|diff|compare files line by line|
|du|estimate file space usage|
|echo|display a line of text|
|find|search for files in a directory hierarchy|
|fg | resumes suspended jobs and bring them to the foreground|
|grep | print lines matching a pattern|
|kill | send a signal to a process|
|less | read file with pagination|
|ln | create links|
|ls | list directory contents|
|lsb_release | print distribution-specific information|
|lsof | list open files|
|mkdir | create|
|mv | move files|
|nc | arbitrary TCP and UDP connections and listens|
|netstat | print network connections, routing tables, interface statistics...|
|nice | execute a utility with an altered scheduling priority|
|nproc | print the number of processing units available|
|passwd | change user password|
|pgrep | look up processes based on name and other attributes|
|pkill | send signal to processes based on name and other attributes|
|printenv | print all or part of environment|
|pwd | print name of current/working directory|
|top | display Linux processes|
|tr | translate or delete characters|
|ps | report a snapshot of the current processes|
|rm | remove files or directories|
|rmdir | remove directories|
|rsync | remote file copy|
|scp | secure copy (remote file copy program)|
|sed | stream editor for filtering and transforming text|
|sleep | suspend execution for an interval of time|
|sort | sort lines of text file|
|ssh | OpenSSH SSH client (remote login program)|
|ssh-keygen | SSH key generation, management and conversion|
|su | substitute user identity|
|sudo | execute a command as another user|
|tail | output the last part of files|
|tar | manipulate archives files|
|tr | translate or delete characters|
|uname | Print operating system name|
|uniq | report or omit repeated lines|
|uptime | show how long system has been running|
|w | Show who is logged on and what they are doing|
|whereis | locate the binary, source, and manual page files for a command|
|which | locate a command|
|wc | print newline, word, and byte counts for each file|
|xargs | build and execute command lines from standard input|
| \| | redirect standard output to another command|
|~> | redirect standard output|
| < | redirect standard input|
| & | send process to background.|

```\ -> This symbol is called the escape character which allows you to insert certain characters in your text and they will not be interpreted by the shell as command ```
### IMPORTANT SHORCUTS
```
CTRL+A -> go to beginning of line 
CTRL+B -> moves backward one character
CTRL+C -> stops the current command
CTRL+D -> deletes one character backward or logs out of current session
CTRL+E -> go to end of line
CTRL+F -> moves forward one character
CTRL+G -> aborts the current editing command and ring the terminal bell
CTRL+K -> deletes (kill) forward to end of line
CTRL+L -> clears screen and redisplay the line
CTRL+N -> next line in command history
CTRL+R -> searches in your command history
CTRL+T -> transposes two characters
CTRL+U -> kills backward to the beginning of line
CTRL+W -> kills the word behind the cursor
CTRL+Y -> retrieves last deleted string
CTRL+Z -> stops the current command, resume with fg in the foreground or bg in the background
```
# SHELL TUTORIALS PROPER
#### WHAT IS SHELL
Shell takes commands from the keyboard and give them to the operating system to perform. Shells are known as command line interface. CLI's

For Study and clarity sake we will be learning with the unix system (Linux). In the shell a program called BASH (Bourne Again SHell) is used in written commands to the computer system. Theere are other programs called KSH, TCSH & ZSH these are also on the availbale on the Linux systems. It is important to note that the BASH is the enhanced version of the former version of the unix shell program SH.

#### A TERMINAL
This is a program that opens a window and lets you interact with the shell. There are many terminals though like the gnome-terminal, konsole, xterm, rxvt, kvt, nxterm, and eterm they are all included in some Linux distributions.

In shell there is availablity for command history. this was inserted to help users not to repeat the process of typing the commands over and over again. It is expedient to know that when you handle this command history, once the terminal closes the history is lost.

#### NAVIGATION
There are 3 basic commands used in navigating the linux environs
- CD: which means Change Directory
- PWD: which means Print Working Dir (note that DIR is same thing as Directory)
- LS: which means List files and Directories.

#### FILE SYSTEM ORGANIZATION
* The files of a linusx system is arranged in what is called Hierarchical Directory Structure. They are organised like a tree.
* Linux system does no use drive letters to indicate location of directories like in windows.
* It is expidient to note that "One important difference between Windows and Unix-like operating systems such as Linux is that Linux does not employ the concept of drive letters. While Windows drive letters split the file system into a series of different trees (one for each device), Linux always has a single tree. Different storage devices may be different branches of the tree, but there is always just a single tree".

#### PWD (PRINT WORKING DIRECTORY)
The 'pwd' Command allows you to print the current working directory. it is very important because it helps us know exactly where we are in the linux system.
  * To use this command we simply type: 'pwd' then Press enter on the keyboard.

#### CD (CHANGE DIRECTORY)
The 'cd' command is used to change working directory either forward or backward depending on where you want to be at a given time.
This command is typed followed by the pathname we would like to move in or the directory we would like to work in.
"A pathname is the route we take along the branches of the tree to get to the directory we want; There are two pathnames that can be specified
* Absolute Pathnames: They begin with the root directory and then follows branch by branch until the path to the diretory desired is completed.
* Relative Pathnames: They start from the working directory and they use special notations to represent relative positions in the file system tree. (."Dot" .."Dot Dot")
```
cd /usr/bin - a typical example of absolute pathname
cd . or cd .. - a typical example of relative pathname
```
It is expedient to note that the (dot dot) allows you to return one directory backwards to the parent directory. You can return to a previous directory by using an absolute pathname like
```
"cd /usr 'This is good if you still know the name of the directory you are returning to.
```
You can also move into a directory with the relative pathname.
```
cd ./bin (this eludes everyother step and moves into the directory named.
```
Take Note: Though Linux supports long file names which may contain embedded spaces and punctuation characters, limit the punctuation characters to period, dash, and underscore. Most importantly, do not embed spaces in file names. If you want to represent spaces between words in a file name, use underscore characters. You will thank yourself later.
#### LS (LIST)
This command lists the name of files and directory in a working directory this means, if we are in an active directory called 'Smart" and there are directories in them with some files, the only way to know them is by listing them with a special notation.
	* ls -a
This command lists the name of directories and files but also lists the hidden files and directories also.
# LOOKING AROUND
We will be looking into certain commands that will help us access certain things on the linux system.
* LS (list files and directories)
* LESS (view test files)
* FILE (Classify a file's contents)

#### LS (LIST)
This command is used to list contents of a directory.
The 'LS' can be used in different ways but to mention a few here are they.
| COMMAND | RESULT |
| ------- | ------ |
| ls      | List the files in the working directory |
| ls /bin | List the files in the /bin directory (or any other directory that needs to be specified) |
| ls -l | List the files in the working directory in long format |
| ls -l /etc /bin | List the files in the /bin directory and the /etc directory in logn format |
| ls -la . . | List all files (even ones with names beginning with a period character, which are normally hiddem) in the parent of the working directory in long format. |
```
Some commands  use extra arguments to handle certain issues like:
command -options arguments, a typical instance is this command:
"ls -l .."
Where command is the name of the command, -options is one or more adjustments to the command's behavior, and arguments is one or more "things" upon which the command operates.
```
#### LESS
This a program that allows you view text files in the linux enviroment.
* Computers do not understand text files or documents, they only understand numbers and so they use certain systems to display text contents to humans, one of such is called the ASCII (AS-KEY). It is said to be an acronym for  "AMERCIAN STANDARD CODE for INFORMATION INTERCHANGE".
	It is expedient to know that text is a simple 1 to 1 mapping of characters to numbers. twenty characters of text translates to twenty bytes of data.

The less command is invoked by simply typing:
``` less text_file```
This means LESS is the command and "TEXT_FILE" is the name of the text_file you want to view its text content.

imagine having a file named 'Notes_from_school' and you want to view its contents, the simple way to do it is by typing the less command to display the contents of the file.

#### CONTROLLING THE LESS DISPLAY
Less displays text contents in pages and this makes it possinle to handle its display in a simple form.
To control the contents of the less file you will have to use certain buttons like:
'PAGE UP KEYS' and the "PAGE DOWN KEYS'. this allows you move through the pages 
When we want to exit the text page we press 'Q'.
Here is a list of options on how to use the 'Less' Command.
| COMMAND | ACTION |
| ------- | ------ |
| Page Up or b | Scroll back one page |
| Page down or space | Scroll forward one page |
| G | Got ot the end of the text file |
| 1G | Go to the beginning of the text file |
| /Characters | Search forward in the text fil for an occurence of the specified characters |
| n | Repeat the previous search |
| h | Dispaly a complete list less commands and options |
| q | Quit. |

#### FILE ####
File command, examines a file and tells us what kind if file it is. 
``` file name_of_file```
Files that are recognised by the 'File command'
* ASCII text
* Bourne-Again Shell Script Text
* ELF 64-bit LSB executable
* ELF 64-bit LSB shared object
* GNU tar archive
* gzip compressed data
* html document text
* JPEG image data
* PostScript document text
* Zip archive data

*_IN LINUX THERE ARE NO SECRETS_*

#### NOTE: ####
There are strange files in the linux enviroment that are called "Symbolic Links".
_Symbolic Links_ are a special type of file that points to another file.

#### MANIPULATING FILES
One may ask why cant i use the GUI (Graphical User interface) to solve my command problems but the truth is that using the command line allows you to exercise your power and flexibilty.
In manipulating files there are certain commnads that helps us get those issues resolved; Commnads like: CP, MV , RM and MKDIR

 - CP: this means Copy files and Directories
 - MV: Move or rename files and directories
 - RM: Remove files and directories
 - MKDIR: create Directories.

_These are meanings for basic commands used for manipulating files and directories._
*WILDCARDS*: they are special characters whihc allows to selecte file-names based on patterns of characters. Here are summary of wildcards and their meanings:
| *Wildcard* | *Meaning* |
| ---------- | --------- |
| * | Matches any characters |
| ? | Matches any single character |
| [characters] | Matches any character that is a member of the set characters. The set of characters may be expressed as a POSIX (*Portable Operating System Interface*).|
|	| | ---------- | ---------- | [:alnum: |

### FINDINGS
- Did you know that: The commnad for checking how many lines you have in a file is "wc -l 'file name'".
- The commnad to check the heading of a file is "head -n 1 'file name'".

# Do You Know
```
mv /test/master /test/my_test_dir: The 'mv' is the _move-command_ then followed by the _directory-name_ this is is where the file will move from ' ' a space is given then the command is completed by inserting the _dir_ of the _dir_ where the file is expected to be placed.

* mv-the move command.
* /test-first directory.
* /master-the second dir where the file is leaving from.
* - the space allows you to start another section of the same command.
* /test-the second directory which indicates where the file is going.
* /my_test_dir - the last destination for the moved file.

all this well placed will produce the expected result of moving a file from one directory to another.
```

### SOMETHING TO ADD
```
#!/bin/bash

# Create a symbolic link from source_file to destination_file
source_file="/path/to/source/file"
destination_file="/path/to/destination/file"

ln -s "$source_file" "$destination_file"

echo "Symbolic link created!"
```
-> In this example, you need to specify the source_file variable with the path to the file you want to create a symbolic link for, and the destination_file variable with the desired path and name of the symbolic link.

The ln command with the -s option is used to create a symbolic link. The "$source_file" represents the source file, and "$destination_file" represents the destination where the symbolic link will be created.

After running the script, it will create a symbolic link from the source_file to the destination_file, and you will see the "Symbolic link created!" message printed on the terminal.
