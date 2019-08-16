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
