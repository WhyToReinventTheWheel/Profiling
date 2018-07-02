# Profiling
Java cpu and memory profiling

# Check Java Process
>jps
4052
5784 Jps
6552 Main
8092 Launcher
> “jstack PID >> mydumps.tdump“
> jcmd PID Thread.print.   // java8

# Thread Dump Details 
Thread Name: Name of the Thread
Thread Priority: Priority of the thread
Thread ID: Represents the unique ID of the Thread
Thread Status: Provides the current thread state, for example RUNNABLE, WAITING, BLOCKED. While analyzing deadlock look for the blocked threads and resources on which they are trying to acquire lock.
Thread callstack: Provides the vital stack information for the thread. This is the place where we can see the locks obtained by Thread and if it’s waiting for any lock.
