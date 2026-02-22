# LINUX SYSTEM PERFORMANCE& PROCESS MANAGEMENT
____________________________________________________________________________________________________________________________________________
## I have documented this file to help master process management,CPU,memory,and I/O monitoring.
____________________________________________________________________________________________________________________________________________
# Prerequisites
* Launch Amazon Linux Instance
* Install the required tools 
* Sudo yum install -y htop iotop sysstat stress-ng
____________________________________________________________________________________________________________________________________________
# Part 1:Understanding Processes
A process is a running program.When you start a program the OS creates a process for it.
## Every process has:
* A process ID (PID)-unique identifier
* Parent PID-Who started the process
* User-Who owns the process.
* State-Sleeping,running,stopped,zombie
* Priority-How important a process is 
* Recources-CPU,memory that a process is using
____________________________________________________________________________________________________________________________________________
#View All processes 
## See all proceses
**Ps aux**
#Explanation of output:
* USER-Who owns the output
* PID-The process ID.
* %CPU-CPU usage percentage
* % MEMORY-Memory Usage precentage.
* VSZ-Virtual memory size(kb)
* RSS-Physical memory used(kb)
* TTY-means no terminal
* STAT-Process status
* START-When the process started
* TIME-Total time used
* COMMAND-What is running
  ________________________________________________________________________________________________________________________________________
  # Example output breakdown
  |User|PID|%CPU|%MEM|VSZ|RSS|TTY|STAT|START|TIME|COMMAND|
  |:----:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
  |root|1|0.0|0.1|19692|1604|?|Ss|10🕥|0.01|/sbin/init|
