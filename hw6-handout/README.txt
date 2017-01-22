Programming 6 (Doubly Linked Lists)

Files you won't modify:
   dll_pt-test.c0 - Test for doubly-linked lists with a point
   elem_char.c0 - Defines dll element type to be char

Files you will modify:
   dll_pt.c0 - Doubly-linked lists with a point

==========================================================

Testing in coin
   % coin -d elem-char.c0 dll_pt.c0 function-tests.c0
   --> test_dll();

Compiling and testing dll_pt:
   % cc0 -d -o dll_pt-test elem-char.c0 dll_pt.c0 dll_pt-test.c0
   % ./dll_pt-test
   Visualizing the text buffer with elem as char.
   Give an initial input for the buffer (empty line quits): foo
   Initial buffer: START <--> 'f' <--> 'o' <--> _'o'_ <--> END
   Give actions (empty line quits): <^^
        START <--> 'f' <--> 'o' <--> _'o'_ <--> END
   <= : START <--> 'f' <--> _'o'_ <--> 'o' <--> END
   del: START <--> 'f' <--> _'o'_ <--> END
   del: START <--> _'f'_ <--> END
   ...
 
==========================================================

Submitting:
  
  Copy the file dll_pt.c0 to your handin directory on WesFiles
