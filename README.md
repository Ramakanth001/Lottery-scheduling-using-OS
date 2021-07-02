# Lottery-scheduling-using-OS
Lottery scheduling is a probabilistic scheduling algorithm for processes in an operating system. Processes are each assigned some number of lottery tickets, and the scheduler (CPU) draws a random ticket to select a process and this random withdrawal continues till all the processes burst time is exhausted.

**Problem:**
In the problem we have to assign one or more lottery tickets to each of the process. A lottery ticket is chosen at random, and the process holding that ticket gets the CPU. The operating system implements lottery scheduling by holding a lottery 50 times each second, with each lottery winner getting 20 milliseconds of CPU time (20 milliseconds × 50 = 1 second). Hence the quantum time is 1sec.

**Solution:**
According to the problem, first we allocate Burst time and Priority for each process. One or more lottery ticket is assigned to each of the process. Assign more tickets to the higher priority process. The probability of completion of process with more number of tickets increases. Random ticket is generated and process having the ticket gets the CPU for the specified quantum time. After the quantum time, the running process is preempted and another random ticket is generated. Now the process with the ticket gets the CPU. This process will continue until all the processes are completed.
 
**Main Concept:**
Ticket allocation takes place considering 2 major factors, Burst time and allocated priority. Realtively more tickets will be allocated to higher priority process so that ultimately the process with more priority has more chances of being chosen in lottery. 
