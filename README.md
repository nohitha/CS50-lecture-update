# CS50-lecture-update

# Completed watching week 0 lecture.
# Note points
# What is Computer Science?
* The input, black box and out put.
* Binary digits representation:
* 1 byte = 8 bits
* Representation of data
* ASCII- alphabets,putuations and other symbols.
* letters with accent marks,emojis are part of unicode. Unicode use more bits than ASCII.
* image binary representation with pixels of RGB.
* videos can be a lot of images dispalyed one after the other.(number of frames per second)
* Music represented by notes, volume, duration.
# ALGORITHMS
* Example in a phone book searching for Mike Smith.
* Pseudocode, functions, conditions, boolean expressions and loops.
# SCRATCH
* variable - the ability to store values and change them
* threads - the ability for our program to do multiple things at once
* events - the ability to respond to changes in our program or inputs
# Completed pset0 and submitted
* Fairy, Princess and ghost(animation) in scratch.
# Completed watching week 1 lecture
# C Language
* hello world program
* compilers - source code to machine code
* clang filename.c to compile and ./a.out to execute.
* 2nd method - clang -o name name.c and ./name for execution.
* ls, cd, mkdir, pwd, rm filename(to remove), cp sourcename destinationname(to copy), mv sourcename destinationname(to change file name)
* strings
* comparing scratch block with c code 
* variables, conditions - if, if-else,nested if-else, loops - while,do while, for.
# Types, format specifer and operators
* int, bool, float, double,long,char,string - types.
* get_int, get_float,get_double, get_char,get_string,get_long -> cs50.h library also include bool.
* %c - char,%s - string,%i - int,%li - long,%f -float,double -> format specifiers.
* +, -,/,%,* ->operators.
* Few examples - age in number of days, price printed with tax,parity(even or odd),conditions, agree(y or Y, N or n),cough 3 times within a function also prototype or declaration of function after predefined libraries and before main.
* get_positive_integer only as input -> use do while for input.
# Screens
* to print ???? -> which is a part of representation in mario game.
* to print square wall as in mario game.
# Memory, imprecision and overflow
* Computer has memory, in hardware chips called RAM. Programs use that RAM to store data as they run, but that memory is finite. So with a finite number of bits, we can’t represent all possible numbers (of which there are an infinite number of). So our computer has a certain number of bits for each float and int, and has to round to the nearest decimal value at a certain point.
* float value output after decimal can be any number of digits, but you can specify number of digits to be represented after decimal by %.4f for 4 digits after decimal.
* EXAMPLES: 
* 1. X = 1, Y = 10, Then computer output of X/Y = 0.10000000149011611938476562500000000000000000000000
