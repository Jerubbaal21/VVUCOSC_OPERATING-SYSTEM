# VVUCOSC_OPERATING-SYSTEM

# Memory Management Algorithm In Operating SYSTEM
- Memory management is the functionality of an operating system which handles or manages primary memory and moves processes back and forth between main memory and disk during execution. Memory management keeps track of each and every memory location, regardless of either it is allocated to some process or it is free.

## Multiprogramming with a fixed number of tasks
- MFT (Multiprogramming with a Fixed number of Tasks) is one of the old memory management techniques in 
which the memory is partitioned into fixed size partitions and each job is assigned to a partition. The memory 
assigned to a partition does not change. 

## Multiprogramming with a variable number of tasks
- MVT (Multiprogramming with a Variable number of Tasks) is the 
memory management technique in which each job gets just the amount of memory it needs. That is, the 
partitioning of memory is dynamic and changes as jobs enter and leave the system. MVT is a more ``efficient'' 
user of resources. MFT suffers with the problem of internal fragmentation and MVT suffers with external 
fragmentation.

## FIRST-FIT METHOD, WORST-FIT METHOD AND BEST-FIT METHOD
- One of the simplest methods for memory allocation is to divide memory into several fixed-sized partitions. Each 
partition may contain exactly one process. In this multiple-partition method, when a partition is free, a process is 
selected from the input queue and is loaded into the free partition. When the process terminates, the partition 
becomes available for another process. The operating system keeps a table indicating which parts of memory 
are available and which are occupied. Finally, when a process arrives and needs memory, a memory section 
large enough for this process is provided. When it is time to load or swap a process into main memory, and if 
there is more than one free block of memory of sufficient size, then the operating system must decide which 
free block to allocate. Best-fit strategy chooses the block that is closest in size to the request. First-fit chooses 
the first available block that is large enough. Worst-fit chooses the largest available block.

## Paging Technique Of Memory Management
- In computer operating systems, paging is one of the memory management schemes by which a computer stores 
and retrieves data from the secondary storage for use in main memory. In the paging memory-management 
scheme, the operating system retrieves data from secondary storage in same-size blocks called pages. Paging is a 
memory-management scheme that permits the physical address space a process to be noncontiguous. The basic 
method for implementing paging involves breaking physical memory into fixed-sized blocks called frames and 
breaking logical memory into blocks of the same size called pages. When a process is to be executed, its pages 
are loaded into any available memory frames from their source.

## a) FCFS   
- For FCFS scheduling algorithm, read the number of processes/jobs in the system, their CPU burst times. The 
scheduling is performed on the basis of arrival time of the processes irrespective of their other parameters. Each 
process will be executed according to its arrival time. Calculate the waiting time and turnaround time of each of 
the processes accordingly.

## b) SJF 
- For SJF scheduling algorithm, read the number of processes/jobs in the system, their CPU burst times. Arrange 
all the jobs in order with respect to their burst times. There may be two jobs in queue with the same execution 
time, and then FCFS approach is to be performed. Each process will be executed according to the length of its 
burst time. Then calculate the waiting time and turnaround time of each of the processes accordingly.

## c) Round Robin (pre-emptive)
- For round robin scheduling algorithm, read the number of processes/jobs in the system, their CPU burst times, 
and the size of the time slice. Time slices are assigned to each process in equal portions and in circular order, 
handling all processes execution. This allows every process to get an equal chance. Calculate the waiting time 
and turnaround time of each of the processes accordingly.

## d) Priority
- For priority scheduling algorithm, read the number of processes/jobs in the system, their CPU burst times, and 
the priorities. Arrange all the jobs in order with respect to their priorities. There may be two jobs in queue with 
the same priority, and then FCFS approach is to be performed. Each process will be executed according to its 
priority. Calculate the waiting time and turnaround time of each of the processes accordingly.

## Multi-level Queue Scheduling Algorithm
- Multi-level queue scheduling algorithm is used in scenarios where the processes can be classified into groups 
based on property like process type, CPU time, IO access, memory size, etc. In a multi-level queue scheduling 
algorithm, there will be 'n' number of queues, where 'n' is the number of groups the processes are classified 
into. Each queue will be assigned a priority and will have its own scheduling algorithm like round-robin 
scheduling or FCFS. For the process in a queue to execute, all the queues of priority higher than it should be 
empty, meaning the process in those high priority queues should have completed its execution. In this 
scheduling algorithm, once assigned to a queue, the process will not move to any other queues.

## Bankers Algorithm
- In a multiprogramming environment, several processes may compete for a finite number of resources. A process 
requests resources; if the resources are not available at that time, the process enters a waiting state. 
Sometimes, a waiting process is never again able to change state, because the resources it has requested are 
held by other waiting processes. This situation is called a deadlock. Deadlock avoidance is one of the techniques 
for handling deadlocks. This approach requires that the operating system be given in advance additional 
information concerning which resources a process will request and use during its lifetime. With this additional 
knowledge, it can decide for each request whether or not the process should wait. To decide whether the 
current request can be satisfied or must be delayed, the system must consider the resources currently available, 
the resources currently allocated to each process, and the future requests and releases of each process. 
Banker???s algorithm is a deadlock avoidance algorithm that is applicable to a system with multiple instances of 
each resource type.



