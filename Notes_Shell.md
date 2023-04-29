# SMART GRABS BELOW
### HOW TO CHANGE YOUR NAME FROM THE COMMAND LINE TO GITHUB
```
git config user.name "New Name"
```
### SOME WORKABLE COMMANDS NEEDED FOR PERFORMANCE IN SHELL
```
awk # pattern scanning and processing language
basename # strip directory and suffix from filenames
bg # resumes suspended jobs without bringing them to the foreground
cat # print files
cd # change the shell working directory.
chmod # change file mode
chown # change file owner and group
crontab # maintain crontab files
curl # transfer a URL
cut # remove sections from each line of files
date # display or set date and time
dig # DNS lookup utility
df # report file system disk space usage
diff # compare files line by line
du # estimate file space usage
echo # display a line of text
find # search for files in a directory hierarchy
fg # resumes suspended jobs and bring them to the foreground
grep # print lines matching a pattern
kill # send a signal to a process
less # read file with pagination
ln # create links
ls # list directory contents
lsb_release # print distribution-specific information
lsof # list open files
mkdir # create
mv # move files
nc # arbitrary TCP and UDP connections and listens
netstat # print network connections, routing tables, interface statistics...
nice # execute a utility with an altered scheduling priority
nproc # print the number of processing units available
passwd # change user password
pgrep # look up processes based on name and other attributes
pkill # send signal to processes based on name and other attributes
printenv # print all or part of environment
pwd # print name of current/working directory
top # display Linux processes
tr # translate or delete characters
ps # report a snapshot of the current processes
rm # remove files or directories
rmdir # remove directories
rsync # remote file copy
scp # secure copy (remote file copy program)
sed # stream editor for filtering and transforming text
sleep # suspend execution for an interval of time
sort # sort lines of text file
ssh # OpenSSH SSH client (remote login program)
ssh-keygen # SSH key generation, management and conversion
su # substitute user identity
sudo # execute a command as another user
tail # output the last part of files
tar # manipulate archives files
tr # translate or delete characters
uname # Print operating system name
uniq # report or omit repeated lines
uptime # show how long system has been running
w # Show who is logged on and what they are doing
whereis # locate the binary, source, and manual page files for a command
which # locate a command
wc # print newline, word, and byte counts for each file
xargs # build and execute command lines from standard input
| # redirect standard output to another command
~> # redirect standard output
< # redirect standard input
& # send process to background
```
### IMPORTANT SHORCUTS
```
CTRL+A # go to beginning of line
CTRL+B # moves backward one character
CTRL+C # stops the current command
CTRL+D # deletes one character backward or logs out of current session
CTRL+E # go to end of line
CTRL+F # moves forward one character
CTRL+G # aborts the current editing command and ring the terminal bell
CTRL+K # deletes (kill) forward to end of line
CTRL+L # clears screen and redisplay the line
CTRL+N # next line in command history
CTRL+R # searches in your command history
CTRL+T # transposes two characters
CTRL+U # kills backward to the beginning of line
CTRL+W # kills the word behind the cursor
CTRL+Y # retrieves last deleted string
CTRL+Z # stops the current command, resume with fg in the foreground or bg in the background
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
#
| Tasks | Files | Description |
| ----- | ----- | ------ |
| 0: Authors/README File | [AUTHORS](https://github.com/justinmajetich/AirBnB_clone/blob/dev/AUTHORS) | Project authors |
| 1: Pep8 | N/A | All code is pep8 compliant|
| 2: Unit Testing | [/tests](https://github.com/justinmajetich/AirBnB_clone/tree/dev/tests) | All class-defining modules are unittested |
| 3. Make BaseModel | [/models/base_model.py](https://github.com/justinmajetich/AirBnB_clone/blob/dev/models/base_model.py) | Defines a parent class to be inherited by all model classes|
| 4. Update BaseModel w/ kwargs | [/models/base_model.py](https://github.com/justinmajetich/AirBnB_clone/blob/dev/models/base_model.py) | Add functionality to recreate an instance of a class from a dictionary representation|
| 5. Create FileStorage class | [/models/engine/file_storage.py](https://github.com/justinmajetich/AirBnB_clone/blob/dev/models/engine/file_storage.py) [/models/_ _init_ _.py](https://github.com/justinmajetich/AirBnB_clone/blob/dev/models/__init__.py) [/models/base_model.py](https://github.com/justinmajetich/AirBnB_clone/blob/dev/models/base_model.py) | Defines a class to manage persistent file storage system|
| 6. Console 0.0.1 | [console.py](https://github.com/justinmajetich/AirBnB_clone/blob/dev/console.py) | Add basic functionality to console program, allowing it to quit, handle empty lines and ^D |
| 7. Console 0.1 | [console.py](https://github.com/justinmajetich/AirBnB_clone/blob/dev/console.py) | Update the console with methods allowing the user to create, destroy, show, and update stored data |
| 8. Create User class | [console.py](https://github.com/justinmajetich/AirBnB_clone/blob/dev/console.py) [/models/engine/file_storage.py](https://github.com/justinmajetich/AirBnB_clone/blob/dev/models/engine/file_storage.py) [/models/user.py](https://github.com/justinmajetich/AirBnB_clone/blob/dev/models/user.py) | Dynamically implements a user class |
| 9. More Classes | [/models/user.py](https://github.com/justinmajetich/AirBnB_clone/blob/dev/models/user.py) [/models/place.py](https://github.com/justinmajetich/AirBnB_clone/blob/dev/models/place.py) [/models/city.py](https://github.com/justinmajetich/AirBnB_clone/blob/dev/models/city.py) [/models/amenity.py](https://github.com/justinmajetich/AirBnB_clone/blob/dev/models/amenity.py) [/models/state.py](https://github.com/justinmajetich/AirBnB_clone/blob/dev/models/state.py) [/models/review.py](https://github.com/justinmajetich/AirBnB_clone/blob/dev/models/review.py) | Dynamically implements more classes |
| 10. Console 1.0 | [console.py](https://github.com/justinmajetich/AirBnB_clone/blob/dev/console.py) [/models/engine/file_storage.py](https://github.com/justinmajetich/AirBnB_clone/blob/dev/models/engine/file_storage.py) | Update the console and file storage system to work dynamically with all  classes update file storage |