## Lab 2 - Command Lines
To test these command Lines use a terminal such as Windows Terminal, Gitbash, or Msys2
## $ hostname
The command hostname will print the systems DNS name. When called without arguments the command will print out the current system name. For instance my host name is DESKTOP-PL9I9BC
## $ env
The env command allows you to display your current environment or run a specified command in a changed environment. If no flags or parameters are specified, the env command displays your current environment, showing one Name=Value pair per line.
## $ ps
The ps command allows you to check the status of active processes on a system, as well as display technical information about the processes
## $ pwd
The pwd command allows you to write the standard output of the full path anme fo your current directory. These directories are all seperated by a slash moving left to write for directory (folder) hierarchy. 
## $ git clone https://github.com/kevinwlu/iot.git
The git clone command uses the gitbash command clone to copy a repository online to your computer. In this instance it copies Kevin W lu's github repository iot from the link https://github.com/kevinwlu/iot.git . This is very useful for organizing projects. 
## $ cd iot
The terminal command cd (curretn directory) tells you which folder the terminal path is set to. To modify this add an argument after cd as follows " cd filename ". The file for filename must be in your current directory or folder. This can be used to navigate to diffent directories. In this instance the terminal will make iot the current directory. 
## $ ls
The ls terminal command allows you to view the files and folder in your current directory. ls stands for list. 
## $ df
The df terminal command allows you to displays the information of your computer. The device name, total blocks, total disk space, used disk space, available disk space, and mount points on a file system.
## $ mkdir demo
The mkdir demo allows you to make a new directory (folder) with the name of the argument you pass in. In this instance the folder is called demo. This is useful for creating folders in the terminal.
## $ cd demo
This terminal command builds on the previous commands. Because when you make a directory using mkdir, the directory is made in your current path. You do not need to branch to the folder its in because you are already in it. " cd demo " allows you to enter into demo. 
## $ nano file
The nano file command opens the nano editor. Nano is a line based code editor that allows you to edit files from the terminal. 
## $ cat file
The cat file command allows you print in standard output the file parameter to the terminal. You can additionally inlcude a dash " - " for standard input. 
## $ cp file file1
The cp terminal command allows you copy a file from a location and write it to a directory. Additionally as viewed in the above instance, it can be used to copy and write one file to another. The contents of file will be copied to file1. 
## $ mv file file2
The mv command allows you to move a file to different file paths. In this instance file will be moved to file2 or into the same path of file. If there is already a file with that name the file will add a 2 after it. 
## $ rm file2
The terminal command rm allows you to remove a non-directory type file that the command calls. In this case, file2 is that non directory type file and file2 will be removed from its current path. This can be useful when moving or replacing files in the terminal.  
## $ clear
The clear command clears the terminal of all previously written commands. It will clear the terminal windows and any output that is generated from them. 
## $ man uname
The man terminal command displays the manual page for a command. In this case the terminal command is asking for the manual page of uname. uname is the command for displaying the name and version of the running operating system as well as additional information such as processor type and hostname. 
## $ uname -a
As previously mentioned the uname command will provide information about the system. When an additional argument is prompted, the output will change. In this instance the command will output a series of information including system kernel name, network node hostname, system release version, system version, machine hardware name as well as the operating system name and version. 
## $ ifconfig
The terminal command ifconfig assigns an address to a network interface for the ability to configure or display the current network interface configuration information. 
## $ ping localhost
The terminal command ping allows you ping a server or network with the address. This has been configured to ping the localhost, essentially pining your computer.
## $ netstat
The netstat terminal command will print in standard form statistics about your active networks. This will provide the status of your protocols. 
