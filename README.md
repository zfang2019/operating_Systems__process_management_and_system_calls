# Operating Systems: Process Management and System Calls
## Part 1: System Call tracing

### Part 1 (a): 
Your first task is to modify the xv6 kernel to print out a line for each system call invocation. Please note no new system call has to be added for this part. Print the name of the system call and the number of times it has been called in the following format:

<System Call Name>  <count>
eg:
sys_fork 10

The system calls issued on booting the xv6 and the number of times they are called, is same all the time. Hence, your implementation should print the same sequence every time. Expected output can be seen in the file out_assig1_1 for reference purposes. We will use some other hidden test cases, whose output will different to make sure that the implmentation is correct and not just a bunch of printf statements.

### Part 1 (b): Add sys_toggle() system call
After you are done with the part a of the assignment, every time you boot or issue some command, you will see system trace printed on the screen, which makes it difficult to see the output of some other command. Hence, as part b, you will have to implement, a sys_toggle() system call, which will toggle the system trace. If it is ON, it will switch it OFF, and vice versa. By default, when xv6 boots, it should be ON.


## Part 2: sys_add() System Call

In this part you have to add a new system call to xv6. This system call should take two integer arguments and return their sum.
You should add a system call named, sys_add() to xv6 and then create a user-level program to test it. You can use user, program provided by us which is called assig1_3.c that calls your new system call.


## Part 3: sys_ps() System Call

In this part you have to add a new system call sys_ps(), to print a list of all the current running processes in the following format:
pid:<Process-Id> name:<Process Name>
...
...
eg:
pid:1 name:init

Similarly for this part, create a new user program, which should in turn call your sys_ps() system call, or you can use assig1_5.c provided by us.
