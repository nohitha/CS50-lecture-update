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
# Completed watching week 1 lecture (C lang)
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
# Completed watching week 2 lecture (Arrays)
# Compiling
* It includes -> preprocessing(loading pre defined library into code), compiling(source to assembly), assembling(instructions to binary), linking(links all binary code).
# debugging
* Bugs are mistakes in program which we did not intend to make.finding and fixing bugs is debugging.
* we can use help50 make name.c, debug50 ./name (add breakpoint or indicator and then debugg), check50, style50.
* Datatypes, Memory
# Arrays
* array stores similar data in continious memory.
* casting -> eg: float a = 1.2 can be casted to integer by -> (int) a
* array example programs: average of 3 scores.
# Strings
* string is an array of characters which ends with '\0'.
* string.h library has strlen().
* ctype.h has toupper()
# Command line arguments
* int argc and string argv[] are arguments passed to take an input while execution.
* where argc -> no. of arguments and argv[] -> is the input.
* Eg: ./hello has argc 1 and argv[0], ./hello nohitha has argc of 2 and argv[0] is ./hello and argv[1] is nohitha.
# Readability
* we can analyze paragraphs of text for their level of readability, based on factors like how long and complicated the words and sentences are.
# Encryption
* Encryption is defined as -> plain text(input msg) ->encrypt using key -> cipher text (msg to destination).
* Eg: plain text (HI! -> 72 73 33) -> encrypt key be 1 -> cipher text (IJ" -> 73 74 34).
# Completed week 3 lecture (Algorithms)
# Searchings
* Linear search -> O(n), omega(1)
* Binary search -> O(log n), omega(1)
# BigO
* BigO means "on the order of". The number of steps taken to solve or runtime. (worst case)
* omega -> the least no of steps taken to solve or run algorithm (best case).
# Structs
* user can define this datatype which contain different datatypes which are of linked information.
* syntax is similar to this example below: 
  typedef struct 
  { 
  string name;
  string number;
  } person;
* declaration in main: type name -> eg: person people[4];
* to access elements of struct in main() person.name[index] or person.number[index].
# Sortings
* Bubble sort -> O(n^2), omega(n)
* Selection sort -> O(n^2), omega(n^2)
* Insertion sort  -> O(n^2), omega(n)
* Merge sort -> O(nlogn), omega(nlogn)
* Finally, there is another notation, Θ, Theta, which we use to describe running times of algorithms if the upper bound and lower bound is the same. For example, merge sort has Θ(n log n) since the best and worst case both require the same number of steps. And selection sort has Θ(n2).
# Recursion
* When a function or algorithm refers to itself.
* In the lecture, took an example of marion pyramid.
* eg:factorial
# Completed week 4 lecture (Memory)
# Hexadecimal
* The address of memory use representation of 16 digits with 0-9 then A-F in hexadecimal.
* RGB color system also conventionally uses hexadecimal to describe the amount of each color. 
* we prefix hexadecimal with 0x as to differentiate 0010 in hexadecimal and 10 in decimal system.
# Pointers
* In C -> & operators means get the address of this variable.
* %p where p is pointer. pointer -> is the address of a variable,points to a location in a memory.
* Pointer is represented as *. The * operator mean go to the location that a pointer is pointing to.
* Eg: printing *&n, to declare and use pointer *t = &a.
# strings
* the CS50 Library defines a string with typedef char *string. we can take string type as char * or a pointer to a character.
* We can also try printf("%p\n", &s[0]).Can also replace s[0], s[1], and s[2] actually which map directly to *s, *(s+1), and *(s+2).
# Compare and copy
* eg: compare values print same or different, make first letter of string to uppercase.
* string.h -> strlen(), strcmp, strcpy and more.
# valgrind
* when we allocate memory using "malloc" then "free" the memory when remained  unused.So that freed memory can be used again.
* If we keep on allocating memory using malloc but didn't freed after using it leads to memory leak -> It slows down the computer and use more and more memory until the computer runs out of memory.
* valgrind is a command line tool to check memory leaks. -> help50 valgrind ./filename
* http://valgrind.org/docs/manual/quick-start.html#quick-start.prepare 
* sizeof gives no. of bytes
* bufferoverflow -> where we go above the buffer size, array size and unknown memory. eg: a[3] -> using a[3] or a[4] causes overflow.
# Swap
* to swap two variables we need 3rd variable.
* when swap function is called with 2 paramaters passed, the copy of those variables are passed and then swappedin that function, but not the original values in main.
* to change original values use call by reference that means passing an address and using pointer.
# Memory layout
* there are different sections in memory.
* first one is machine code which is compiled binary code, located at top in the memory.
* next, global variables
* then heap area -> whenever we call malloc the heap area grows towards bottom.
* last stack area -> whenever we call main or any other function in main then sack area grows upward.
* when we call many times malloc -> heapoverflow. when we call main many times -> stackoverflow. these 2 types of overflow are bufferoverflow which may cause program to crash.
# scanf
* to take input from the keyboard.
* eg: scanf("%i", &x);
# files
* eg: phonebook to append name and mobile number which produce csv file, to read name and mobile number from phone book.
* fopen, fclose, fprintf to print the file. fread to read the file.
# jpeg
* eg: to check that input is jpeg or not. clue: always first 3 bytes in jpeg are 0xff 0xd8 0xff.
# Problem pset 2
* one problem completed and submitted. readability to check the grade -> finding words, letters, sentences applying on  formula.
* caesar problem -> to encrypt the text using valid key.
# problem pset3
* plurality -> more no. of votes to a candidate, then print the candidates name.
* runoff -> to find who wins in election by runoff method.


