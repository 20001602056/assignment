# Introduction
In this section we will try to understand various linux basic commands, file tree and linux ssh.

---
# Assignments
---
--- 
# BASIC COMMANDS
---
## cd
### Must Do
* Goto `/` root of linux directory using cd command.
* Goto `home` directory of user
* Goto two directories back using single command.
* Goto previous directory wuthout using `cd ../` command.
---
## ls
### Must Do
* List only files whose extension is **log or gz** in **/var/log** directory
* List files in **/var/log** sorted by the order of last modified time
* List files in accordance to the size of file in ascending order.

### Good to Do  
* To open the last edited file in the current directory use the combination of ls, head and vi commands as shown below.  
* Display file size in easy to read format. i.e M for MB, K for KB, G for GB.  
---
## head & tail
### Must Do
* List top 10 lines of **/var/log/auth.log**
* List last 10 lines of **/var/log/auth.log**
* Keep on listing new content appended to **/var/log/auth.log**
### Good to Do
* List the content of **/var/log/auth.log** from line number 10 till 20
---
## grep
### Must Do
* List out all the lines in **/var/log/auth.log" containing this content **session opened for user root**
* Create a file that will have multiple name, post that find users have a specific last name. i.e. If I want to find users have lastname "Rawat" and if the file contains Mukesh Rawat it should be listed down
* List all the lines of /etc/passwd that ends with “bash” word.
* List the user whose name is of 5 character long.
### Good to Do
* Find out users who have login shell as **/bin/bash**
---
## du and df
### Must Do
- Check the size of any directory which is present on my system.
- Check the size of subdirectories in a directory.
- List out all the devices which is currently mounted in my system.
- List how much resource mounted resources are using.

### Good to Do
- List the sub directories of a directory which are more than 5 mb.
- List the mounted devices which are mounted in **/dev**
---
## top and ps
### Must Do
- List out top 10 process which is using high memory.
- List out the process of current user
- Start the firefox browser and kill the process of firefox.
- Evaluate when we have to kill the process forcefully and what are the methods.

### Good to Do
- Set firefox priority as most prior process.
---
## netstat and telnet
### Must Do
- List out the ports which are listening.
- Check the ssh port accessiblity from another server.
---
## env and export
### Must Do
- List out the current environment variables
- Set a env in linux which is `CODE=NINJA`

### Good to Do
- Add env variables in env files.

---
## Cut
### Must Do
- Displays 2nd character from each line of a file.
- Extracts first 3 characters of each line from a file.    
- extracts from 3rd character to end of each line from file.
- Displays only first field of each lines from /etc/passwd file using the field delimiter : (colon). In this case, the 1st field is the username.


### Good to Do
- Extract the second field of the class file and redirect standard output to the file class.lastname. 

---
## find
### Must Do
- Find all the files whose name is fresher.txt in a current working directory.
- Find all the files whose name is fresher.txt and contains both capital and small letters in /home directory.    
- Find all php files whose name in a current working directory.
- Find all Executable files.
### Good to Do
- To find all hidden files.  
- To find and remove multiple files such as .mp3 file.  

---
## tr
### Must Do
- Change all text from lower case letters in text to upper case in file .
- Find all the files whose name is fresher.txt and contains both capital and small letters in /home directory.

### Good to Do
- Here is an example of breaking a single line of words (sentence) into multiple lines, where each word appears in a separate line.
- Translate multiple lines of words into a single sentence.  

---
## sed
### Must Do
- using sed one-liner will return lines 5 through 10 from any text file.
- Display lines 5-7 and 10-13 from myfile.txt  
- To replace every instance of the word "road" with "rd" in myfile.txt.

### Good to Do
- Here is an example of breaking a single line of words (sentence) into multiple lines, where each word appears in a separate line.
- viewing the authorization and authentication activities that took place on July 2, as per the /var/log/secure log.
- Let’s suppose you have a file containing full names in the format First name, Last name. To adequately process the file, you may want to switch Last name and First name using sed command.  

---
## awk
### Must Do
- Print only Specific field like 2nd & 3rd.  
- Write A Command To Rename The Files In A Directory With "_new" As Postfix.
- To Find The Total Number Of Lines In A File Without Using Nr.  
- produce the Fibonacci series using the awk command

### Good to Do
- write an awk script to delete all the files of directory that are older than the given time provided in minutes.
- write an awk script to print the no of lines in each file in the given directory.
- you will get an input as 5 columns each containing a number you have to print the max and min sum that can be gained by adding four columns. 

## References
---
https://www.howtogeek.com/117435/htg-explains-the-linux-directory-structure-explained/

---

--- 
# LINUX FILE TREE
---
## Must Do
- Login to the terminal and change directory to root ie. `/`
- List out all the directories.
- Find the binaries of `ls,cp,cat,lsblk,which` commands.
- Find the binaries of `lvm,swapon,swapoff,iptables` commands.
- Execute this command `whereis rsyslog.d`, and go to each directory showed in stdout and summarize what kind of files are present in those directories. 
- Summarize the reason why there are different directories and their significance.
	- `/var/log`
	- `/home`
	- `/var`
	- `/etc`
	- `/bin`
	- `/proc`

## Good to Do
- Identify the path variables in your shell and their significance. 
- Find out the significance of rest of the directories.

## References
* https://www.howtogeek.com/117435/htg-explains-the-linux-directory-structure-explained/
---

--- 
# LINUX ssh(Secure Shell)
---

## Must Do
- Setup two machine and perform ssh between them by both method password method and ssh-key method.
- Use verbose mode with ssh and summarize your understanding.
- Change the default port of ssh.
- Copy a text file from one server to another using **scp**

## Good to Do
- When ssh connection is setup, restrict user to a particular directory and its sub-directories.
---
## References
* https://www.hostinger.in/tutorials/ssh-tutorial-how-does-ssh-work#gref
---

--- 
# RUNLEVEL
---
## Must Do
- Change the default boot runlevel by editing the appropriate file.
- Alter the current runlevel WITHOUT rebooting the system.
- Observe and display the runlevel.
- Change the runlevel back, observe and display the new runlevel information

## Good to Do
- Check if nginx and openssh-server installed and start the nginx service before ssh service start.
---

## References
---
* [Runlevels and rcd](https://www.linux.com/news/introduction-services-runlevels-and-rcd-scripts)
---

--- 
# TEXT PROCESSING
---
---
### Problem 1
* write an awk script to print the no of lines in each file in the given directory 
---
### Problem 2
* You will get an input having n number of rows and 2 column you have to find the sum of the difference of each column.
---
### Problem 3
* you will get an input having n number of rows and 2n number of columns each row will contain odd column as string and even column as number if number is greater than 10 than print the string on previous column.  
Sample Input  
test 1 testa 11  
testb 12 testc 9  
sample 12 samplea 89  
sampleb 8 samplec 34 sampled 1  
Sample Output  
testa  
testb  
sample  
samplea  
saplec  

---
### Problem 4
* write an awk script to delete all the files of directory that are older than the given time provided in minutes.
---
### Problem 5
* Task
You are provided a file with four space-separated columns containing the scores of students in three subjects. The first column, contains a single character (A-Z) - the identifier of the student. The next three columns have three numbers (each between 0 and 100, both inclusive) which are the scores of the students in English, Mathematics and Science respectively. Your task is to identify the performance grade for each student. If the average of the three scores is 80 or more, the grade is 'A'. If the average is 60 or above, but less than 80, the grade is 'B'. If the average is 50 or above, but less than 60, the grade is 'C'. Otherwise the grade is 'FAIL'.Input FormatThere will be no more than 10 rows of data. Each line will be in the format: [Identifier][Score inEnglish][Score in Math][Score in Science] Output Format For each row of data, append a space, a colon, followed by another space, and the grade. Observe the format showed in the sample output.  
Sample Input  
A 25 27 50  
B 3537 75  
C 75 78 80  
D 99 88 76  
Sample Output  
A 25 27 50 : FAIL  
B35 37 75 : FAIL  
C 75 78 80 : B  
D 99 88 76 : A  

Explanation A scored an average less than 50 => FAIL
Same for B  
C scored an average between 60 and 80 => B  
D scored an average between 80 and 90 => A  

---
### Problem 6
* You are provided a file with four space-separated columns containing the scores of students in three subjects. The first column, contains a single character (A-Z) - the identifier of the student. The next three columns have three numbers (each between 0 and 100, both inclusive) which are the scores of the students in English, Mathematics and Science respectively.
Input Format
There will be no more than 10 rows of data. Each line will be in the format:
[Identifier]<space>[Score in English]<space>[Score in Math]<space>[Score in Science]  
Output Format  
Concatenate every 2 lines of input with a semi-colon.  
Sample Input  
A 25 27 50  
B 35 37 75  
C 75 78 80  
D 99 88 76  
Sample Output  
A 25 27 50;B 35 37 75  
C 75 78 80;D 99 88 76  

---
### Problem 7
* you will get an input as 5 columns each containing a number you have to print the max and min that can be gained by adding those columns

## References
* https://likegeeks.com/awk-command/
---

--- 
# USER MANAGEMENT
---

## Must Do
- create a user test1 using useradd  
- create a user test2 using adduser  
- compare their entries in /etc/passwd file and /etc/shadow file  
- add a new group named testGroup  
- add test1 and test2 to that group using usermod  
- make test1 to be able to login to system and work like normal user  
- remove user test1 and test2  
- remove group testGroup  

## Good To Do
- you will be given a csv file containing name, group, shell, home dir for n user. Create a shell script to add those user with provided configuration.  
- also give them a unique default password so that they can login to their with that password and change it later  
---
## References
* https://www.tecmint.com/manage-users-and-groups-in-linux/
---

--- 
# FILE PERMISSION
---
## Must Do
- Create a shell script for hello world with name tycoon.sh via root user
- Verify the permission of tycoon.sh
- Execute the script, if it didn't get executed give appropriate permissions for root user.
- Switch to normal user and execute tycoon.sh, if it didn't get executed give appropriate ownership to user (do not change the owner of file)
- Move tycoon.sh to a path variable use it as a binary ie invoke it from anywhere.

## Good to Do
- Learn about SUID, SGID and sticky bit.
- And Set if for a dummy file.
- Explore how SUID, SGID is used for ***passwd***.
---

## References
---
* https://www.thegeekdiary.com/understanding-basic-file-permissions-and-ownership-in-linux/
* https://www.tutorialspoint.com/unix/unix-file-permission.htm
---

--- 
# PACKAGE MANAGEMENT
---
### Must Do

* Locate and explore the directories containing repository definitions.
* Practice enabling and disabling epel repository in Centos system.
* Install httpd2.4/apache2.4 using its .rpm/.deb file.
* Use the package manager to install php7.2 and its dependencies.
* Use the package manager to uninstall php7.2 and its dependencies.
* Note packages and make a list of their dependencies, install and run them.
* Perform operations to find, view and remove the specific packages.

### Good to Do

* Manipulate packages and repositories
* Installs portmaster and uses it to update installed ports.
* Install nodejs 10.x using source code.
* Install and setup MySQL 5.7 in non interactive mode.

## References
* http://www.informit.com/articles/article.aspx?p=2118682&seqNum=3
---

--- 
# PROCESS MANAGEMENT
---
## Must Do
- Display all the users processes
- Highlight running processes in top and sort the processes in descending order of CPU utilisation and close the application with  highest CPU utilisation.
- System is running multiple processes and among which one process is transferring files over the remote system, how do I will give this process the highest priority.
- Kill all the process of external users logged in to the system.
- Shows the child-parent hierarchy of all processes
- What are signals and List all of the signals that can be sent to a proccess
- List out the status of background jobs
- Resume (wake up) a suspended process with PID 6436 but keeps it running in the background
- Shows how long a particular process was running. 
- lists all open files belonging to processes owned by the user 
- Kill all process that belongs to a particular user
- Display the process ID numbers of the zombie processes.


## Good to Do
-  List out all system calls used for process management and write a short description on it with the example on the implementation.
---

--- 
# CRON
---

## Must Do
- Have clear understanding of all crontab fields.
- Create 2 users such that one user can setup cron and other can't.
- Create a file that holds the information whenever the system boots.
- Clear cache of your system every 2 hours between 10am to 8pm daily.
- Append current system timestamp in file every 15 seconds.

## Good To Do
- Rotate system log file every 35 minutes using crontab.
- Send a broadcast message to all logged-in users every 2nd and 4th monday of a month at 3pm

## References
* [Linux Crontab](https://www.educba.com/linux-crontab/)
---

--- 
# DISK MANAGEMENT 
---
## Must Do
- List all available disk devices on the system .
- Explore disk device names and where they exists on the filesystem.
- Use the fdisk partition tool to create two partitions on your pen drive.
- Mount those partitions persistently on the system.
- Add quota options to the mounted partitions.

## Good to Do
- Create a user for assigning a disk quota.
- Configure quota on the intended filesystem.
- Create a soft and hard limit quota for space on the created use.
- Forcibly exceed those quotas and observe the results.
- Generate a quota report on system users.
---

## References
---
* https://www.binarytides.com/linux-command-check-disk-partitions/
* Disk Quota](https://www.linux.com/learn/step-step-using-user-quotas-linux
---

--- 
# INODE MANAGEMENT
---
## Assignments
## Must Do
- create a file File1 and found it's inode number
- change the inode no of File1
- change the permission of File1 and add some content in File1 using the inode no of File1
- find out the total no of inodes assigned to your file system
- create a directory dir_1,make a hard link and soft link of dir_1
- list out all the links of directory "/"
## Good To Do
- checkout the inode usage of your filesystem if it's more than 50% then delete all the files whose size is less than 10 kb but before deleting the files copy the content of the files in final_data.log.
- now simulate this problem for a directory Sample_Dir which will act as our dummy file system.Sample_Dir will have multiple directories and all the directories will have multiple files of any size.
- write a script for this problem.

## References
* https://linoxide.com/linux-command/linux-inode/
---

--- 
# Logical Volume Manager (LVM)
---
## Must Do
- Crystal clear understandng of PV, VG and LV.
- Create LVM 2 partitions on Pen drive with space left for two more to create.
- Create physical volumes of the 3 partitions created.
- Create volume group of the physical volumes.
- Create logical volumes and mount on system persistently.
- Extend the LVM partition created earlier.

## Good to Do
- Reduce the LVM partition created earlier.
- Take snaphot of LVM and restore it

## References
* https://www.tecmint.com/create-lvm-storage-in-linux/
---

--- 
# SYSTEM RESOURCE MANAGEMENT
---

## Must Do

- Run a program with modified scheduling priority.
- Print network connections, routing tables, interface statistics, masquerade connections, and multicast memberships.
- Check System Load Average.
- Report a snapshot of the current processes.
- Display system tasks.
- Create a user for assigning a disk quota.
- List all available disk devices on the system .
- Display virtual memory statistics

## Good to Do

- check the ram used by the system if the ram exceeds by 40% then Stop the process which has maximum disk utilization.
- Investigate information about successful logins and tracks the activities of valid users.

---
