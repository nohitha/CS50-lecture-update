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
* X = 1, Y = 10, Then computer output of X/Y = 0.10000000149011611938476562500000000000000000000000
* It turns out that this is called floating-point imprecision, where we don’t have enough bits to store all possible values, so the computer has to store the closest value it can to 1 divided by 10.
* i = 1, i is multiplied by 2,infinite number of times. sleep(1) available in unistd.h library.
* We see the number gets bigger and bigger until 1073741824 and prints an error integer overflow then it turns to 0.
* As it could not store next value it displayed error. But still doubling it gives a negative number and then continues printing 0.
* This problem is called integer overflow, where an integer can only be so big before it runs out of bits and “rolls over”. We can picture adding 1 to 999 in decimal. The last digit becomes 0, we carry the 1 so the next digit becomes 0, and we get 1000. But if we only had three digits, we would end up with 000 since there’s no place to put the final 1!
* Examples: Y2K calender year representing 99 instead of 1999 later found bug and took more memory to rectify problem.
* A Boeing 787 has a bug that counter in the generator overflows. so it should be restrated or rebooted and set counter to 0 again.
# Completed pset1 and submitted
* hello world program.
* mario -> left spaces + right triangle wall.
* cash -> greedy problem. print least minimum coins to be given to the customer.
# Completed watching week 2 lecture
# Compiling
* It includes -> preprocessing(loading pre defined library into code), compiling(source to assembly), assembling(instructions to binary), linking.

