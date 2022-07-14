# linux-basics
Notes for necessary linux commands 


		                    	Getting started with Linux
What is Linux?
Linux is an open source operating system. It is free to use.
It is secure.
It is customizable.
It is a top choice of developers.

Flavors of Linux

Linux has  many  distributions  and versions of the operating system. Some of the widely used and famous  flavors of linux are Ubuntu, Fedora, Mint, Debian, openSUSE etc.

Linux File Hierarchy Structure

<img src = "linux file structure-1.jpg">
The Linux File Hierarchy Structure or the Filesystem Hierarchy Standard (FHS) defines the directory structure and directory contents in Unix-like operating systems.
In the FHS, all files and directories appear under the root directory /, even if they are stored on different physical or virtual devices.
 – The Root Directory
Everything on your Linux system is located under the / directory, known as the root directory. You can think of the / directory as being similar to the C:\ directory on Windows – but this isn’t strictly true, as Linux doesn’t have drive letters. While another partition would be located at D:\ on Windows, this other partition would appear in another folder under / on Linux.

Linux in DevOps

Infrastructure Automation is amongst the major practices done in most IT companies. Linux is highly used in the domain of infrastructure automation.
With Linux’s help, you can save time through instance creation and increase the efficiency of operations.

Some of the important Linux commands.
1.	 ssh
Connecting to EC2 instance with the terminal command
ssh -i file.pem username@ip-address
ssh: Command to use SSH protocol
-i : Flag that specifies an alternate identification file to use for public-key authentication.
username: Username that uses your instance
ip-address: The IP address is given to your instance

2.	 ls
Listing directory contents
ls
The default output of the ls command shows only the names of the files and directories. Use the -l to print files in a long listing format:
ls -l 
The ls command doesn’t list the hidden files by default. A hidden file is any file that begins with a period (.).to display all files, including the hidden files, use the -a option:
ls -a


3.	 pwd
Present working directory
Use the pwd command to find out what directory you are currently in:
pwd

4.	 cd
Changing directory
When used without any argument, the cd will take you to your home directory:
cd
you can use either relative path or absolute path to change your pwd
here is an example to navigate to your downloads folder
cd /Users/Mrigesh/Downloads 
if your pwd is /Users/Mrigesh , just type
cd Download 
To go back to the previous directory
cd ../
To move two levels up
cd ../../
To change back to the previous working directory, use the dash (-) character as an argument
cd –

5.	 cat
Displaying file contents.
cat /Users/Mrigesh /Downloads/linux.txt

6.	 touch
Creating  file
touch file.txt

7. vim
Editing content
vim file.txt

7.	 rm
Removing files and directories
Removing  empty  file
rm file.txt
Removing  empty directory 
rm -d directoryname
To remove non-empty directories and all the files within them recursively, use the -r
rm -rf directoryname

8.	 cp
The cp command allows you to copy files and directories
To copy a file in the current working directory, use the source file as a first argument and the new file as the second:
cp abc.txt xyz.txt
To copy a file to another directory, specify the absolute or the relative path to the destination directory. When only the directory name is specified as a destination, the copied file will have the same name as the original file.
cp abc.txt /Users/Mrigesh/Downloads

9.	 mv
The mv command is used to rename and move files and directories from one location to another.
For example, to move a file to a directory, you would run:
mv abc.txt /Desktop

10.	 sudo
Elevate privileges
The sudo command allows you to run programs as another user, by default the root user. If you spend a lot of time on the command line, sudo is one of the commands that you will be using quite frequently.
#some examples
sudo apt update 
sudo apt install ansible -y
sudo cat /temp/

12. usermod
Adding users to groups
To add an existing user to a group, use the usermod command followed by the -G option and the name of the group:
usermod -a -G Docker Jenkins 


𝗰𝗵𝗺𝗼𝗱  command
It let's you change the permission of the file. It has a lot of options, the most I used was 𝘤𝘩𝘮𝘰𝘥 +𝘹 𝘧𝘪𝘭𝘦.𝘹 which added the execute flag. Basic permissions:

r (read)
w (write)
x (execute)

𝗴𝗿e𝗽 command
I think grep is really powerful, when working with text files. It searches for lines that match a regular expression. This really helped navigating large log files.




