# 430help -- An MSP-EXP430G2 Pipeline For Dinguses

Because I am a dingus and keep forgetting how to compile and upload files to
my beloved MSP-EXP430G2 Launchpad, I'm building this silly little repository for
myself and for dinguses like myself that need a little help once in a while
remembering how to do stuff... because dingus.

## How to compile MSP430-GCC Programs With the MSP-EXP430G2 launchpad

In the terminal:
```
$ msp430-gcc -Os -Wall -g -mmcu=msp430g2553 <file name.c> -o <file name>.o
$ mspdebug rf2500
```
In mspdebug (after compiling above):
```
(mspdebug) prog <file name>.o
(mspdebug) exit
```
NOTE: mspgcc will do the compiling for you assuming that mspdebug and msp430-gcc
are both installed and that you are using the msp430g2553 with the
MSP-EXP430G2 launchpad.
