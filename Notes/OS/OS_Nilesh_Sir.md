# OPERATING SYSTEM - LINUX PROGRAMMING
 
- Docker is an Linux Kernel
- All the advance software made by you are deployed on the Linux OS.
- You can see that there is no GUI when you are going to deploy your software.
- All the operations must be performed in the Command Line.
- Ultimately all of your applications are going to be deployed on the Linux platform.
- We must know how to operate the Linux server using the commands.
- Nodejs is light weight which means Nodejs is single threaded language.
- You must know about how to create threads in java, c# etc.
- If you want to create the process at the OS level then how to do that.
- If you want to create the thread and process at the OS level then OS provides you with some kind of functions which are called as system calls.
- System calls are the functions exposed by the Kernel-OS, so that the user can access the KERNEL functionalities.
- How to create a file and manipulate the files using the system calls.
- Programs never runs on Hard disk.
- How the RAM is managed behind the scene.
- How pagination and swapping works.
- You can also go through the Sunbeam Section-B Operating System section to cover up the basics.
- CCEE majority of the questions are based on Linux commands.
- Rest of the concept are shell script , linux system calls and conceptual questions.

## What is Operating System 
- Operating system is the interface between the user and the hardware.
- As a end user we deal with the programs and programs deal with the operating system and operating system deals with the hardware.
- Where hardware means Input/Output Device, CPU, RAM, hard disk and management of these hardware is responsibility of OS.
- Kernel is core component of OS.
- Kernel is the CORE Operating system or minimal OS which performs basic minimal functionalities.
- **OS functionalities** : minimal 5 requirements performed by every core OS where core os means Kernel
    - Process management
    - File & Input/Output management
    - Memory management
    - CPU Scheduling 
    - Hardware Abstraction
- **Extra functionalities**
    - user interfacing
    - networking
    - protection
    - security
- Linux is inherited from UNIX OS where UNIX was developed by Dennis Richie and Ken Thomson in 1971.
- To abstract the hardware and provide the functionalities of hardware to rest of the layers we use the HAL i.e Hardware Abstraction Layer.
- UNIX Operating System is based on two pillars : 
    - File control sub-system
    - Process control sub-system
- The Slogan of UNIX is **"Process have lives and Files have spaces"**.
- Everything inside the UNIX OS is either of type file or type process inside UNIX OS.
- Everything is a file according to UNIX including the directory, data, pipe, socket, links, devices which are dealing or sending the data character by character (char devices - keyboard, mouse, serial port, parallel port ) , or (block device - pen drives, hard disk or all storage devices) the devices which are sending the data block by block are also files.
- All the storage devices are block level device where all the data are stored, manipulated sector by sector where 1 sector is equals to 512 bytes. Whenever you read something from pen drive you are reading one sector and whenever you writing on pen drive, you writing  one sector.
- You can never write one byte in the pen drive as it is not designed like that. Whenever you will write in the pen-drive it will always be sector by sector.
- Jab bhi data write hota hai to sector wrote hota hai and jab bhi data read hota hai toh ek sector read hota hai.
- Jo kuch bhi dikhta hai wo files and jo kuch bhi chalta hai wo process.
- Human body is the file and the human soul is process.
- Your whole UNIX is standing on two pillars process control sub-system and file control sub-system.
- In process control sub-system it includes 
    - process and their scheduling
    - threads and their scheduling
    - If there are multiple processes then IPC i.e inter process communication comes into the picture
    - If there exists processes then how the memory is allocated to them also come into the picture.
- In file control sub-system it includes
    - All the input/output management
        - let it be character devices
        - let it be block devices
        - files which are saved using the editor, ide, vs code etc are managed by file control sub-system
- How does programs creates files , processes and threads ?
    - Everything is done using the functions provided by the OS and those are system calls.
    - System calls are the functions that are exposed by the KERNEL, so that the user using those system calls can access the KERNEL functionalities.
    - If you talk about the JVM used in JAVA, CLR used in MS .Net all these does not have the access to the hardware and these are going to run on the top of OS only. Behind the scene JVM and CLR are making the system call internally to OS.


## Linux Architecture
- There are several layers in the Linux Kernel Operating system
    - Process Management
        - Process and thread operations
        - CPU Scheduler works
        - Context Switching
        - CPU hardware is involved
    - Memory Management
        - If there are multiple processes and threads then they will require memory.
        - Memory manager is required to allocate some memory
        - RAM hardware is involved 
    - File Systems
        - There are different file system types : 
            - NTFS , FAT, FAT16, Extended FAT (Windows File System)
            - EXT3 , EXT4 ( Linux File System)
            - Block devices
    - I/O Management and Network Management
        - Character Devices
        - Unlike UNIX, Network are treated separately
        - Network are considered as special type of devices.
- User can access any of the following functionalities using System calls


- System calls are internally called with the help of Software Interrupts internally which helps you to switch between the user mode and kernel mode. This is the typical way how kernel execute the system calls.

- You must become the end user of OS to learn any OS.
- You must know about the commands and shell scripts.
- After becoming the end user. Now, try to become the Administrator of the OS by learning the shell scripts.
- Become the programmer, i.e programmer of OS, you must be good at handling the system calls.
- OS Developer, OS Designer, explore the OS internals.

## Linux Shell
- Shell is a program that inputs the command from the end user and get them executed from the kernel . It is also referred as **command interpreter**.
- Shell is taking the input from the user and giving that input command to the kernel using the system call so that it get executed by the Kernel.
 
- Linux have variety of Shell :
    - bsh/bash
    - csh/tcsh
    - zsh
    - ksh
- Bash shell 
    - Compatible with bsh/sh

- **Linux Command**
```sh
# This will print information about the Linux Operating system you are using.
# Which Linux you are using and also tells about the information of Linux Kernel
terminal > uname -a

# This is the command to list down the directories and files inside it
terminal > ls

# This will list down all the directories and files with their permission and date created and who is the author of the file 
# etc.
terminal > ls -l

# This will list down the directories and files with all the information and the total size of current directory is consuming in mb in human readable format.
terminal > ls -l -h

```

