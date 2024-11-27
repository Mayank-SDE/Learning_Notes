# Operating System
## What is Operating System ? 

- A program that acts as an intermediary between a user if a computer and the computer hardware.
- Operating System goals : 
    - Execute user programs and make solving problems easier.
    - Make the computer system more convenient to use.
- Use the computer hardware in an effiecient manner.

## Computer System Structure
- **Hardware** - provide basic computing resources
    - CPU, memory, I/O devices
- **Operating System**
    - Controls and coordinates use of hardware among various applications and users.
- **Application Programs** - define the ways in which the system resources are used to solve the computing problems of the users.
    - Word processors, compilers, web browsers, database systems, video games
- **Users**
    - People, machines, other computers
 
## Operating SYstem Definition

- OS is a **resource allocator**
    - Manages all resources and
    - Decides between conflicting request for effiecient and fair resource use.
- OS is **control program**
    - Control execution of programs to prevent errors and improper use of the computer.
- Everything a vendor ships when you order an operating system.
- The one program that is running at all times on the computer is the **kernel**. Everything else is either a system program (ships with the operating system) or an application program.

## Instaling OS on PC

## Hard disks
- There are two types of hard disks
    - PATA / IDE
    - SATA
- SATA drivers are faster as copared to PATA drivers.
- These disks are connected to motherboard using different kind of connectors.
- Today's motherboards have one (or more) port's for PATA, while more than four ports for SATA.
- These ports can be used to connect hard disks, CD/DVD R/W or printers.

## Hard Disk Settings 
- The SATA hard disk can be directly connected to motherboard using special SATA cable.
- The PATA hard disk can be connected to motherboard using other type of cable.
- PATA drive must be configured using the jumper settings in one of the following modes : 
    - Primary Master
    - Primary Slave
    - Secondary Masster
    - Secondary Slave

## BIOS settings 

- **Disk configuration**
    - Many of the older OS do not install on Sata disks.
    - For installing such OS, in BIOS, configure disks as IDE or PATA instead of AHCI mode.
- **Boot Options:**
    - Decides the device from which PC should try to boot.
    - The recommended order for boot devices is - 
        - CD/DVD drive
        - Disk Drive
        - USB drive
        - Network boot

## Partitions
- The hard disk can be splt into multiple partitions, so that each partition could be treated as one disk.
- These partitions can be used to install operating systems and to store data/files.
- One disk can have different types of partitions:
    - Primary partition
        - Maximum four can created on a disk.
    - Extended partition
        - Special type of primary partition
        - Onle one etended partition is allowed on a disk.
    - Logical partition
        - Multiple can be created within extended partition.

## File System
- Each partition must have some file system.
- Different operating systems can be installed on different types of files system.
- Example file systems are : 
    - FAT/FAT32 ( WINDOWS OS )
    - NTFS ( WINDOWS SERVER OS )
    - EXT2/EXT3 ( LINUX OS)
    - HFS ( MAC OS )
- FAT or NTFS partitions have drive letters that are used by Windows OS to specify file paths.

## Installing Windows OS 
- Insert Windows OS (Windows XP, Windows 2003 Server, Windows Vista, etc.) CD/DVD into CD/DVD drive and boot from it.
- The Basic OS setup will be loaded into the memory.
- Windows can be installed on first primary partition (OR any primary or logical partition in special case).
- Create first primary partition ( or logical partition ) of appropriate size for the operating system. If the partition are already created then select the partition. The partition will be formatted and OS files will be installed on it.

## Installing Linux System 
- Insert Linux OS (Open SuSE, RHEL,UBUNTU etc) CD/DVD into CD/DVD drive, boot from it and select installation option.
- The basic OS setup will be loaded into the memory.
- Select fresh/new installation option.
- Linux can be installed on any partition.
- Select the Custom Partition Setup and Create appropriate (mostly logical) partition of appropriate size for the OS. If partitions are already created then select from it. The partition will be formatted and OS files will be installed on it.

# System Booting

## Bootable device
- The procedure of starting a computer system by loading the kernel is known as **booting** the system.
- The first sector of any storage device is known as **boot sector**.
- If boot sector of any storage device contains a special program called as **bootstrap program**, then that device is said to be **bootable device**.
- Similarly, if boot sector of the partition of any disk contains this program, partition is said to be a **boot partition**.

## Bootstrap program
- Bootstrap program locates the kernel, loads it into main memory and starts its execution.
- Sometimes two-step process where **boot block** at fixed location loads complex bootstrap program.
- There is a separate bootstrap program for each OS.
- If multiple operating system are installed on the computer, the boot loader encompasses the bootstrap/boot loader for other operating system.
- NTLDR, GRUB, LILO etc are few examples of boot loaders.


## Booting Process
- When computer started, the instructions pointer (program counter) is loaded with a predefined memory location and executions starts there.
- The initial boot program is kept here in ROM, as RAM is in an unknown state at system startup.
- The bootstrap program run diagnostics to determine the state of machine(hardware).
- It also initialize CPU registers, device controllers and such thing so that basic system is initialized.
- It loads kernel of OS from the disk/device to the memory and starts the first process of that kernel.
- Finally one or more system processes are created which functions as an operating system.
