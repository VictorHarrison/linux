#add users on linux system
man page: man useradd

example:
	sudo useradd -m usertest

victor@note-837:~/git-harrison/linux$ cat /etc/passwd | grep usertest
usertest:x:1002:1002::/home/usertest:/bin/sh

	sudo passwd usertest -m

victor@note-837:~/git-harrison/linux$ sudo passwd usertest
Enter new UNIX password: 
Retype new UNIX password: 
passwd: password updated successfully


#usermod

#The usermod command modifies the system account files to reflect the changes that are specified on the command line.



#Linux system has mkhomedir_helper to creat a home diretory to user tha haven't this

sudo mkhomedir_helper usertest
	

