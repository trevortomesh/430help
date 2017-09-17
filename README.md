How to compile MSP430-GCC Programs With the MSP-EXP430G2 launchpad

In the terminal:
$ msp430-gcc -Os -Wall -g -mmcu=msp430g2553 <file name.c> -o <file name>.o
$ mspdebug rf2500

In mspdebug (after compiling above):
(mspdebug) prog <file name>.o
(mspdebug) exit


NOTE: mspgcc will do the compiling for you assuming that mspdebug and msp430-gcc
are both installed and that you are using the msp430g2553 with the
MSP-EXP430G2 launchpad.
