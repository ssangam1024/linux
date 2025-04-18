Day 1

Unix
* Unix is an operating system developed in the 1960s.
* Over the years, many improved versions—called "flavors"—were created by companies like Red Hat, Ubuntu, and SUSE.

Characteristics of Unix:
* It is free to use.
* It is open source.
* It is FOSS (Free and Open Source Software).
* It supports multiple users at the same time.
* It allows multitasking (running many tasks at once).
* It is user-friendly and supports both CUI (Character User Interface) and GUI (Graphical User Interface).
* It is more secure than the Windows operating system.

Flavors of Unix:
Unix is an open-source operating system. Many different versions, or "flavors," are available, with added features and improvements.

Day 2 

Components of Unix
Unix has two main components:
* Shell
* Kernel

Shell
* The shell is the outer layer of the Unix operating system.
* It reads commands entered by the user.
* It checks if the command is valid and used correctly.
* If everything is fine, it converts (interprets) the command into a form that the kernel can understand.
* The shell acts as a bridge between the user and the kernel.

Kernel
* The kernel is the core part of the Unix operating system.
* It is responsible for executing commands using the hardware.
* It handles memory management and CPU (processor) allocation.
* The kernel acts as a bridge between the shell and the hardware.

Command Execution Flow
* Normal user sees the $ prompt.
* Super user / root user/ admin user  sees the # prompt.
* To switch to the root user, use: sudo -i

[User]  
  ⬇ (Enters a command like 'ls' or 'mkdir')  
[Shell]  
  ⬇ (Checks if the command is valid and correct)  
     ├──If valid → Continue  
     └──If not valid →  
               [Shell shows error message to user]  
               ⬆  
               (Command stops here)  
  
⬇
Valid command continues:  
[Shell]  
  ⬇ (Translates the command into a form the kernel understands)  
[Kernel]  
  ⬇ (Handles the command and communicates with hardware)  
  ⬇ (Manages memory, CPU, and devices)  
[Hardware]  
  ⬇ (Performs the actual task – like listing files)  
[Kernel]  
  ⬇ (Sends the result back to the shell)  
[Shell]  
  ⬇ (Displays the output to the user)  
[User]  

Day 3 

Difference between UNIX and Linux

* UNIX is the original operating system, developed in the 1960s. It's paid, closed-source, and mainly used by big companies.

* Linux is a free, open-source operating system inspired by UNIX. It's used by everyone—from beginners to big tech companies—and runs on all kinds of devices like phones, servers, and computers.

Linux File System :

In Linux, everything is treated as a file. There are different types

1. Normal (Ordinary) Files

These are files that contain data, like text, images, videos, audio, or programs.

Example: notes.txt, photo.jpg

2. Directory Files

These are like folders that hold other files or subdirectories.

In Linux, we call them directories instead of folders.

3. Device Files

In Linux, even hardware devices (like USBs, keyboards, or hard drives) are represented as files.

These special files are located in the /dev directory.

They allow the system to communicate with devices.

How to Check File Type in Linux
Use the command: ls -l

The first character of the output tells you the file type:

Symbol	    File Type	            Description

* "-"     Ordinary file	         Regular file with data (text, image, etc.)
* "d"	          Directory	           A folder that can contain files/subfolders
* "l"	        Symbolic link	         A shortcut pointing to another file
* "c"	    Character device file	     Used to communicate with character-based devices (like keyboards, serial ports)
* "b"	       Block device file	     Used with devices that transfer data in blocks (like hard drives)
* "s"	         Socket file	         Used for communication between processes

Day 4

File System Navigation Commands

* . → Current directory
* .. → Parent directory
* ~ → Home directory of the current user

Linux File System Hierarchy

Linux has a tree-like structure, starting from the root directory:
* / → Root directory (the top-most directory of the Linux file system)
Below are some important subdirectories under /:
1. /bin → Contains essential binary executables (programs) used by all users, like ls, cp, mv.
2. /sbin → Contains system binaries used by the superuser (root) for system tasks, like shutdown, reboot.
3. /etc → Stores system configuration files, like network settings, user accounts, and startup scripts.
4. /tmp → Temporary files. This directory is usually cleared on reboot.
5. /dev → Contains special files that represent devices, like hard drives (/dev/sda) or USBs.
6. /mnt → Temporary mount point for mounting file systems, like external drives.
7. /media → Used for automatically mounted devices, like USB drives or CDs.
8. /opt → Optional software packages and third-party applications are stored here.
9. /lib → Contains shared libraries (like DLL files in Windows) used by programs in /bin and /sbin.
10. /var → Stores variable data like logs, mail, and databases. Data here changes often.
11. /usr → Secondary hierarchy for user programs and data. Includes subdirectories like /usr/bin, /usr/lib.
12. /home → Each user’s personal directory is stored here (e.g., /home/alex).
13. /proc → A virtual filesystem showing system information like running processes, CPU info, etc.
14. /boot → Contains boot files, including the Linux kernel and bootloader configuration.


