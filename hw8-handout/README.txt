
Programming 8 (Compression)

File you will hand in:
   huffman.c0

Data structure instantiations:
   hashtable-client.c0
   pq-client.c0
   stack-client.c0

Data structure libraries:
   lib/hashtable.c0
   lib/heaps.c0
   lib/stack.c0

Data:
   freqs/                 - frequency tables
   texts/                 - texts to compress

Files for the extra credit task:
  unpack.c
  pack.c

Files you don't need to look at:
   Makefile               - A short way to compile; just type make
   main-decode.c0         - Main for decoding
   main-encode.c0         - Main for encoding
   other stuff in lib/

==========================================================

To compile your code with contracts on:
   % make debug
   OR
   % cc0 -d hashtable-client.c0 pq-client.c0 stack-client.c0 lib/*.c0 huffman.c0 main-encode.c0 -o encode
   % cc0 -d hashtable-client.c0 pq-client.c0 stack-client.c0 lib/*.c0 huffman.c0 main-decode.c0 -o decode

To compile your code with contracts on:
   % make

   OR

   % cc0 hashtable-client.c0 pq-client.c0 stack-client.c0 lib/*.c0 huffman.c0 main-encode.c0 -o encode
   % cc0 hashtable-client.c0 pq-client.c0 stack-client.c0 lib/*.c0 huffman.c0 main-decode.c0 -o decode


Encoding a file:
   % ./encode -f freqs/<file> -i texts/<file>

Decoding a file:
   % ./decode -f freqs/<file> -i <bitfile>

==========================================================

For the bonus task:

1) get readfile.c0 from the 'hw' directory on WesFiles, and put it in
your hw3-handout/lib directory, replacing the one that's there.

2) get vocab_ascii.txt from the same place

3) in vocab-main.c0, change read_words to read_chars for both the
vocab_filename and the tweet_filename---these are the only two calls to
read_words in the code.

4) use your code from hw3 to make a frequency file

5) back in hw8, run 'make pack' to compile the C code for pack/unpacking

6) to pack a file, run 

   % ./pack <file>

   This creates <file>.pack

7) to unpack a file, run 
   
   % ./unpack <file>

   This creates <file>.unpack


==========================================================

