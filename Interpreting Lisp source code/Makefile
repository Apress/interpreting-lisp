# file: Makefile                              date: 3-01-2017 
#
# This file is a control file for the
# make program.  It contains the specifications for building the lisp
# executable program, lisp, from the C source file lisp.c using the
# GNU C-compiler on linux.  To build the lisp executable, type 'make
# lisp' after the operating system prompt in the ~knott/lisp/
# directory.

# CFLAGS is a macro for the flags passed to the compiler.
# The flag -g tells the compiler to include debugging information
# in the resulting executable; the flag -O means use the lowest
# level of compiler optimizations.  $(CFLAGS) is not given below.
CFLAGS=-g -O

# CC is a macro for the C-compiler used in compile and link commands.
CC=gcc

# The following line begins with the name of the target (i.e. the file
# to be constructed), lisp.o, and then lists the file(s) on which it
# depends--the C source file lisp.c.  The next line is the command for
# compiling the C source file in order to construct the file lisp.o; the
# flag -c means only compile--do not link--the named C file, and the
# flag -o lisp.o means name the output file lisp.o.
lisp.o: lisp.c
	$(CC) -c -o lisp.o lisp.c

# The following line begins with the name of the target, lisp, which
# is an executable file, and then lists the file on which it
# depends--the object file lisp.o.  The next line is the command for
# linking the object file, lisp.o, and producing the output file,
# lisp.  -lm means link in the math library module.
# What are libraries are included by default, if no libraries
# are explicitly named?
lisp: lisp.o
	$(CC)  -o lisp lisp.o -lm -lc

# end of Makefile











