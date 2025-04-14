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

Day -
