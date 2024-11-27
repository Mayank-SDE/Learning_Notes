# Operating System - CIP
- Operating system is an software that takes control of your machine after it gets turned on. Some basic test happens and after that the control is given to the operating system. OS becomes the incharge of your machine.

- The Application programs in your computer does not directly intereact with the hardware instead OS acts an intermediator between them.
- OS becomes the interface between the Application programs and the hardware.
- Imagine the case where you writing the text on the notepad so now to perform simple tasks like moving the mouse and typing from the keyboard even required the coding to perform these tasks , even for saving the text on the harddisk you have to write the program for it.
- The application development will be night mare for us to write the programs to achieve these simple tasks without the OS.
- So OS provides these basic services and you call them system calls.
- It has system calls for writing data into the hardisk, reading data from the harddisk, moving the mouse, programs for displaying something on the screen and your libraries they work on the top of system calls.
- Using the system calls the application development wil becomes really easy.
- Operating system provides three main features - 
    - Resource Management 
        -  You have limited resources on your machine and multiple process running in your machine ex - FireFox browser, Youtube , Some Desktop application. Now you need a manager to decide which process will be running on your CPU. You have limited ram and multiple process are running into the RAM. You need an manager to decide which process should be loaded into the RAM. Which process must go out of the RAM based on some priority. 
    - Abstraction
        - Your OS abstract the hardware, you do not need to write the assembly or binary code. It provdes the system calls which youcan use in the library and your application development becomes easy.
    - Protection
        - Since you have multiple application running in your system. You have to ensure that one application that is running will not affect the other application running in your system. So, protecting the application from one another and protecting the application fro any kind of malware, you need an manager.

### Example of OS
- **Desktop**
    - Windows  
    - Linux
    - MacOS
- **Mobile** 
    - Android
    - IOS
- There exists many OS, even for printers, and many other devices.

## Types of Operating System 
- 1. Single Tasking
    - These OS are very very basic, they are just loaded in the RAM and does not provide multiple functionalities. 
    - These OS allows only one process to be in the RAM at a time.
    - Single task system are very Inefficient. Because CPU is very fast by nature and it does the task in micro-seconds and illi-seconds and I/O deveices are very very slow. So, if there is process in your memory which is assigned by OS now if there are multiple process are waiting so because of the I/O operations CPU is been idle for very long time where still it is capable of executing multiple processes but due to single tasking system it can do one process at a time and this makes the Single tasking system as ineffecient.
    - Example - MS DOS etc
    - Note - If you want to run something in your computer then it must be put on the RAM of the computer. Because CPU can only talks to the programm and processes which are there in the memory i.e RAM. After putting the program in the RAM it gets converted to the process and after becoming the process it will be assigned to the CPU. 
- 2. Multi-programming and Multi-tasking -
    - Use single CPU to allow multiple processes to run concurrently
- 3. Multi-threading
- 4. Multi-processing