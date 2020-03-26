# BasicThreading Assignment
This program is a very simple demonstration of
thread scheduling. After creating the specified
number of threads, it manages the threads round-
robin fashion (0, 1, 2, .. n-1, 0, 1, 2, ..),
selecting each thread in turn. That selected
thread's function prints a running message at
1-second intervals during its time slice, while
other threads silently loop and wait their
turn. A SIGINT handler sets a running flag to
false, causing the threads to terminate and
thread management to complete. It then waits
for the threads to terminate before exiting.
