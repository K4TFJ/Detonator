# Detonator from the book "Commodore 64 Game Book 2" by Gregg Barnett

KeyscanASM is the machine code that is poked into memory.
Line 50 is the POKE routine 

**50 F0R I = 49152 T0 49287:READ Q:POKE I,Q:NEXT**

and it reads from DATA lines 10100-10160

**10100 DATA 165,197,133,180,169,0,133,179,165,180,201,60,208,4,169,1,133,179,165**
**10110 DATA 180,201,62,208,4,169,1,133,178,165,180,201,12,208,4,169,2,133,178,165**
**10120 DATA 180,201,33,208,4,169,3,133,178,165,180,201,41,208,4,169,4,133,178,165**
**10130 DATA 178,201,1,208,10,173,1,208,206,1,208,206,1,208,96,201,2,208,10,173,1**
**10140 DATA 208,238,1,208,238,1,208,96,201,3,208,22,206,0,208,206,0,208,173,0,208**
**10150 DATA 201,254,144,8,173,16,208,41,254,141,16,208,96,238,0,208,238,0,208,173**
**10160 DATA 0,208,201,2,176,8,173,16,208,9,1,141,16,208,96**

I have made a few comments

Look at the 'improved' file for a smaller and faster version (work in progress... untested as of yet)
There was some uneccesary storing, loading and comparing, so I am attempting to fix that. I dont expect a 
large increase in speed. It is definately smaller, so less to type in once I have the DATA lines ready.

For reference, you can find the book at https://archive.org/details/commodore-64-games-book-2/mode/2up



