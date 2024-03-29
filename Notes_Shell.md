# MY_NOTES

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
```\ -> This symbol is called the escape character which allows you to insert certain characters in your text and they will not be interpreted by the shell as command.
```
### IMPORTANT_SHORCUTS
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
```
less text_file
```
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
```
file name_of_file
```
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
| [characters] | Matches any character that is a member of the set characters. The set of characters may be expressed as a POSIX (*Portable Operating System Interface*).character class such as one of the following:|
| [:alnum:] | Alphanumeric characters |
| [:alpha:] | Alphabetic characters |
| [:digit:] | Numerals |
| [:upper:] | Uppercase alphabetic characters |
| [:lower:] | Lowercase alphabetic characters |
| [!characters] | Matches any character that is not a member of the set characters |

*_Summary of wildcards and their meanings_*
| *Pattern* | *Matches* |
| -------- | --------- |
| * | All Filenames |
| g* | All filenames that begin with the character "g" | b*.txt | All filenames that begin with the character "b" and end with the characters ".txt" |
| Data??? | Any filename that begins with the characters "Data" followed by exactly 3 more characters |
| [abc]* | Any filename that begins with "a" or "b" or "c" followed by any other characters |
| [[:upper:]]* | Any filename that begins with an uppercase letter. This is an example of a character class. |
| BACKUP.[[:digit:]] [[:digit:]] | Another example of character classes. This pattern matches any file that begins with the characters "BACKUP". followed by exactly two numerals. |
| *[!]:lower:]] | Any file that does not end with a lowercase letter. |
*wildcards can be used with any commands that accepts filename arbuments.*

### CP: Copy
This copies a single file but can also copy multiple files also.
```
cp file1 file2
or
cp file... directory
```
This other CP usage that helps
| _Command_ | _Results_ |
| --------- | --------- |
| cp file1 file2 | Copies the contents of file1 into file2. if there is no file2 it is created. |
| cp -i file1 file2 | user is prompted before content is overwritten. |
| cp file1 dir1 | copy file1 contents into the same file name in the named directory. |
| cp -R dir1 dir2 | copy the dir1 contents and if dir2 is not created it creates it or it will create dir1 inside dir2. |

### MV: Move
This command performes double task.
1. it renames and same time.
2. It moves.
this double action is dependant on how the command is been used.
```
To rename a file:
mv filename1 filename2

To move a file:
mv file1... directory
```
| *Command* | *Results* |
| --------- | --------- |
| mv file1 file2 | if file2 does not exist file1 is renamed but if file2 exists then its contents are replaced silently. |
| mv -i file1 file2 | (-i means interactive) this means it will prompt the user before any action |
| mv file1 file2 dir1 | files file1 & file2 are moved to dir1, if dir1 is not in existence an error will be displayed. |
|mv dir1 dir2 | if dir2 does not exist dir1 is renamed and if it does exist dir1 is moved into dir2 |

### RM: Remove
This removes or deletes files and directories.
```
Command to remove a file
rm file
```
The recursive command can also be used.
| *Command* | *Results* |
| --------- | --------- |
| rm file1 file2 | Deletes file1 and 2 |
|rm -i file1 file2 | there is a prompt befoer any file is deleted |
| rm -r dir1 dir2 | dir1 & dir2 are deleted with all the contents in it. |
```

Be careful with rm!

Linux does not have an undelete command. Once you delete something with rm, it's gone. You can inflict terrific damage on your system with rm if you are not careful, particularly with wildcards.

Before you use rm with wildcards, try this helpful trick: construct your command using ls instead. By doing this, you can see the effect of your wildcards before you delete files. After you have tested your command with ls, recall the command with the up-arrow key and then substitute rm for ls in the command.
```

### MKDIR: Make Directory
```
The command to make a directory
mkdir directory
```
### COMMANDS AND WILDCARDS
You can combine commands with wildcards and they are done as follows
| _Commands_ | _Results_ |
| ---------- | --------- |
| cp *.txt text_files | This command will copy all the files in the working directory with '.txt' as its extnsion to a directory called text_files |
| mv dir1 ../*.bak dir2 | This command Move the subdirectory dir1 and all the files ending in ".bak" in the current working directory's parent directory to an existing directory named dir2. |
| rm *~ | Delete all files in the current working directory that end with the character "~". Some applications create backup files using this naming scheme. Using this command will clean them out of a directory. |

# WORKING WITH COMMANDS
You can work with certain commands and they are;
	* Type - Displays information about a command
	* Which - Locates a command
	* Help - Display reference page for shell builtin
	* Man - Displays an on-line command reference.

### What are "Commands?"
Commands are divided into 4 kinds
1. An executable program: these are like files in /usr/bin that we saw earlier. Here binary programs wirtten in C and C++ or programs written in script languages like the Shell, Perl, Python, Ruby etc are found.
2. Built in Commands in shell: these commands are called shell builtins. The *mv* command is a shell builtin.
3. Shell Function: they are shell scripts incorporated inot the enviroment.
4. An Alias: These are commands that we can define ourselves and they are mostly built from other commands.

### IDENTIFYING COMMANDS
_Type: This command is a shell builtin command._ It can be used as follows:
```
type command (this is the command name we would like to examine.)
ANOTHER INSTANCE
type type
type ls
type cp
```
_Which: We use this to locate the exact position of an executable_ It can be used in the following ways:
```
which ls
```
_Which only works for executable programs not aliases and builtins. The reason is that these are substitutes for actual executable programs._

### Getting Command Documentation
_Help: is a command that came with the shell, so using it is so simple_
```
help cd
Which will make it run a complete detail about the command.
You can add -m to change the output format. for instance:
help -m cd
```
