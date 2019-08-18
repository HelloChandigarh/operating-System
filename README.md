# operating-System
Basic notes on operating system
Memory -- > Ram , Harddisk , Registers , Cache 
CPU will pull the program line by line from the memory and will execute it .
any program which CPU want to run should be in ram . Apart from program , there will be data inside ram which the cpu will use .
The data will copied  from harddisk to RAM and then CPU will access it because the access time of ram is kinda million times that of harddisk .

Need of Operating System:
Long term scheduler is a program in operating system which will decide which programs needs to kept inside ram .
Operating system is called as resource manager (any device we use can be called as a resource s ram is a resource and os is allocating programs to ram )
If there are two process in ram and they are competing to access RAM , In that case function in os will decide whcih process will access first . This functionality of OS is called as short term Scheduler.

Whenever we switch on computer the os program will be copied to RAM . the space where the os code is placed as called as OS code space .othe space is called user place where we keep prorgrams .

Input/Output Device : every IO device has a memory buffer where the binary data will go and fro there it will be transferred to RAM and from there it will move to CPU registers and there the operation will be performed (eg calculation will be done in this way usig ALU) the result will be overridden in any of the register and from there it wil move to CPU and cpu will move it to Ouput Register (eg monitor )


PROGRAM will be either executed by CPU or it is performing some IO event or it is waiting for both the operation to happen .

Turn around time : waiting time(it just waited inside cpu) + burst time(execution time) + I/o time (i/o time)
(time taken by program to stay in CPU)


Program Vs Process
in HDD we have googlechrome.exe it is called as program .the running instance of googlecrome is called as process.
States of program:
New state -> Ready State(waiting for CPU or I/o Operation) -> Running state ( being executing by CPU)->I/O state (if performing I/O event, its also called blocked state)-> Terminated state(after execution , removed from ram ) ->Suspend ready state-> Suspend wait state .

Degree of Multiprogramming (maximum number of programs that can be stayed inside ram )

Types of Operating system : 

Degree of multiprogramming is always 1 . Both I/O and CPU will not be working simultaneously for a single process . they can work at the same time for different process . so if one process is runnig we are wasting the resources .So the efficiency is low .

CPU Efficiencey =userful time of CPU /total time of CPU .
out of total time for how much time cpu is getting consumed .

Multiprogramming operating system : more than one program in the ram .it improve efficiency .(if one of the process is undergoing I/O , i can use the other process to consume CPU .It is called concurrent processing .

MultiProcessing OS : we can have more than one CPU .It will improve the efficiency . It is called parallel processing .
we have multiprocessing computers these days .


Passive Entity: A program creating the processes is called passive entity .
Active Entity : the process which is which being used actually is called active entity 

Process Control block :Apart from the program , process  has stack ( in case the program function call each other ) , It has heap(dynamic memory allocation, allocating memory at runtime ) and also memory for global or static variables (in case the program has static and global variables ).

Properties/Attributes of process :
Process ID:Process ID(unique number of every process) ,
program counter(p1,p2,p3 are three processes in ram,os code will decide which one wil be picked by cpu to execute . that os code is called scheduler . there are multiple algorithms to do that . One is first come first serve  like p1 come to ram first than p2 so it will be executed first . there is another one which is called shortest job for scheduling algorithms (one will shortest execution time will be executed first )if we terminated the process in between , to execute some higher priority . progam counter is the line of the program where we terminated . so that again moving to the program which got terminated , from that line we need this .we store the progra counter inside a registers .
General purpose register : every process will . have register values which need to be remembered (incase we reschedule some terminated process ) so it will be kept in gerneral purpose registers.
Priority 
list of open files : list of open files should be remembered . the reading of the left out files after rescheduling should be done 
list of open devices 
protection







