Programming 2 (Images)

==========================================================

Files you will modify:
   pixel.c0           - Replace this with your Programming 1 solution
   imageutil.c0       - Skeleton image helper functions
   nightvision.c0     - Nightvision transform
   rotate90.c0        - Rotate90 transform
   rotate.c0          - Rotate transform
   
Files you won't modify:
   remove-red.c0      - An example transform
   images-main.c0     - Code for running the transforms

Files that don't exist yet:
   imageutil-test.c0  - test your imageutil.c0 (optional)
   
==========================================================

Testing your imageutil:
   $ coin -d imageutil.c0 imageutil-test.c0
   --> main();


Compiling images:

   $ cc0 -d -o transform pixel.c0 imageutil.c0 remove-red.c0 nightvision.c0 rotate.c0 rotate90.c0 images-main.c0
   (You need to do this every time you make changes.)

   OR

   $ make
   (This may not work if you don't have the right cygwin/macports
    package installed.)


Running remove red:
   $ ./transform -t remove_red -i images/gargoyle.png
   (This produces images/gargoyle_remove_red.png, which should be the same
    as images/gargoyle_remove_red_sample.png)

Running nightvision:
   $ ./transform -t nightvision -i images/eiffel.png
     (This produces images/eiffel_nightvision.png, which should be the same
      as images/eiffel_nightvision_sample.png)

Running rotate90:
   $ ./transform -t rotate90 -i images/gargoyle.png
     (This produces images/gargoyle_rotate90.png, which should be the same
      as images/gargoyle_rotate90_sample.png)

Running rotate:
   $ ./transform -t rotate -i images/gargoyle.png
     (This produces images/gargoyle_rotate.png, which should be the same
      as images/gargoyle_rotate_sample.png)

Note that you can also run 

./transform -t <whatever> -i images/gargoyle.png -o images/you-pick-the-file-name.png

if you'd like to specify the output file name.

==========================================================

Creating a tarball to submit on WesFiles:
   $ tar -czvf hw2sol.tgz pixel.c0 imageutil.c0 nightvision.c0 rotate90.c0 rotate.c0

Submitting the tarball:
   There is a directory on WesFiles named
   /courses/COMP-211-dlicata/handin/<yourname>/

   You must upload a file hw1sol.tgz to this directory.

   You can do that on the web by going to 
   https://wesfiles.wesleyan.edu
