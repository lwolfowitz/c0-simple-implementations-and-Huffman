Programming 4 (Clac)

Files you won't modify:
   lib/stacks_int.c0     - Stacks containing integers
   lib/queues_string.c0  - Queues containing strings
   lib/tokenize.c0       - Library for populating queues of strings
   clac-main.c0          - Runs clac

Files you will modify:
   clac.c0               - Clac interpreter

Data:
   def/demo-fail.clac    - An example program that should call to error()
   def/demo-print.clac   - An example program that should print things out

==========================================================

Compiling and running the Claculator:
   % cc0 -d -o clac lib/*.c0 clac.c0 clac-main.c0
   % ./clac
   % ./clac def/demo-print.clac

==========================================================

To handin: 

   Copy clac.c0 to your handin directory on WesFiles

