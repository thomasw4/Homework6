# Process Class

## This class ecapsulates the resources created when spawning a Unix/Linux process with the fork() system call.  It uses the RAII idiom to make usage easier by freeing any 
resources upone object destruction.

Screencasts of this project are available at
http://youtu.be/lTB3kiltIuw
http://youtu.be/L17bVZMxbw0



DISCUSSION
This is a good use of object oriented design.  It provides for easier maintenance and makes the components reusable.  

The process class could allow the user to input an option number to control how the parent and child processes are created and destroyed.  The each option would provide the input to a switch
statement to set timers, alarms, sleep, or delays.  The user could also provide a specific amount of time for execution and destruction.


I believe the SIGCHLD signal can be "listened" for, this could then notify the parent that the child if finished and then start reading data that was written to output
