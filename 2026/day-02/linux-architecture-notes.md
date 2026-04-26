1. The core components of Linux:
Kernel: The heart of linux, it is a program which is written in C language which manages the handware to run process.
User space: It is an environment in which user can perform tasks. E.g. Using ls command to list the files, it uses user space to list.
Systemctl: System controller which controls the user applications. Eg. systemctl start nginx // systemctl stop nginx. 

2. How processes are created and managed?
- Every command that executed by the user in background the kernel gives a process id (PID) which uses specific resources to run that process.
you can use the few commands to manage the existing process-
  I. ps - displays the active process.
  II. kill - kills the process.
  III.htop - displays realtime processes.

3. What systemd does and why it matters?
- Systemd/ init process: Init (Initialization)process the first process started by the kernel after the boot. 
  It is also known as the System Daemon which run in background which is also responsible for launching other process.
