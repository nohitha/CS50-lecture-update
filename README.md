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
# Completed week 5 lecture (Data Structures)
# Pointers
* recap of malloc.
* small video of pointer fun with binky. Initially pointers does not point anything. Pointer pointing to a location is called pointee.
# Resizing arrays
* One solution is to allocate more memory in a larger area that’s free, and move our array there, where it has more space. But we’ll need to copy our array, which becomes an operation with running time of O(n), since we need to copy each of n elements in an array.
* We can use realloc to allocate some more memory for arry extension. realloc copies old array into new one.
# Data Structures
* Data stuctures are programming constructs that allow us to store information in different layouts in our computer’s memory.
* to build data structure we need the below
* struct - to create custom data, . to access properties in structure, * used for pointing to address location.
# Linked Lists
* List can be grown or shrinked.
* values are not stored next to each other in linked list like an array.
* linked list contain nodes, where eac node contain a value and pointer.
* NUL refers to '\0' that means end of string. NULL refers to address of all zeros or null pointing pointing nothing.
* There is no random access unlike an array.
* inserting a node by dynamically allocating more memory. eg: showed an example with students.
# More data structures
* TREE is a data structure where each node points to two other nodes, left (value less than root node)and right (value more than root node)nodes.
* Every node has atmost two nodes. It is called binary search tree. It is a search tree because it’s sorted in a way that allows us to search correctly.
* Run time o search tree is O(logn) and inserting nodes while keeping the tree balanced is also O(logn).
* HASH TABLE: A data structure with constant time search, which is a combination of array and linked list. eg: list of names placed in alpabetic manner by hash code.
* TRIE: It is another data structure.
* Imagine we want to store a dictionary of words efficiently, and be able to access each one in constant time. A trie is like a tree, but each node is an array. Each array will have each letter, A-Z, stored. For each word, the first letter will point to an array, where the next valid letter will point to another array, and so on, until we reach something indicating the end of a valid word. If our word isn’t in the trie, then one of the arrays won’t have a pointer or terminating character for our word. Now, even if our data structure has lots of words, the lookup time will be just the length of the word we’re looking for, and this might be a fixed maximum so we have O(1) for searching and insertion. The cost for this, though, is 26 times as much memory as we need for each character.
* Abstract data structure: they are higher level constructs where we use arrays, linked list, hash table, tries to implement a solution to some problem.
* eg of one abstract data structure is queue (FIFO). insert element -> enqueue, delete element -> dequeue.
* opposite data structure is stack (LIFO). insert an element -> push, delete an element -> pop.
* another eg is dictionary,where we can map keys to values, or strings to values and we can implement with one hash table.
# Completed week 6 (Python)
# Python basics
* Code in python looks simpler than C and also capable of solving data science problems.
* hello world program in python -> print("hello, world")
* No need of standard library, declare a main function, specify a new line in print, use of semicolons like C.
* Python is an interpreted language, means we actually run another program (an interpreter) that reads our source code and runs it top to bottom. For eg: we can save the above as hello.py, and run the command python hello.py to run our code, without having to compile it.
* Eg: answer = get_string("What's your name?\n")
print("hello, " + answer)
* We create a variable called answer, without specifying the type (the interpreter determins that from context for us), and we can easily combine two strings with the + operator before we pass it into print.
* We can also pass in multiple arguments to print, with print("hello,", answer), and it will automatically join them with spaces for us too.
* print also accepts format strings like f"hello, {answer}", which substitutes variables inside curly braces into a string.
* We can create variables with just counter = 0. To increment a variable, we can use counter = counter + 1 or counter += 1.(no ++)
* if x < y:
    print("x is less than y")
elif x > y:
    print("x is greater than y")
else:
    print("x is equal to y")
* Boolean expression:
while True:
    print("hello, world")
* We can write a loop with a variable:
i = 3
while i > 0:
    print("cough")
    i -= 1
* We can also use a for loop, for each element in a list:
for i in [0, 1, 2]:
    print("cough")
* Lists in Python are like arrays in C, but they can grow and shrink easily with the interpreter managing the implementation and memory for us.
* we can use a special function, range, to get some number of values, as in for i in range(3). This will give us 0, 1, and 2, for a total of thee values.
* In Python, there are many data types:
* bool -> True or False
* float -> real numbers
* int -> integers
* str -> strings
* range -> sequence of numbers
* list -> sequence of mutable values, that we can change or add or remove
* tuple -> sequence of immutable values, that we can’t change
* dict -> collection of key/value pairs, like a hash table
* set -> collection of unique values
* docspython.org official source documentation.
# Examples
* We can blur an image with:
from PIL import Image, ImageFilter

before = Image.open("bridge.bmp")
after = before.filter(ImageFilter.BLUR)
after.save("out.bmp")
* implement dictionary
words = set()

def check(word):
    if word.lower() in words:
        return True
    else:
        return False

def load(dictionary):
    file = open(dictionary, "r")
    for line in file:
        words.add(line.rstrip("\n"))
    file.close()
    return True

def size():
    return len(words)

def unload():
    return True
* eg: from cs50 import get_string

s = get_string("What's your name?:\n")
print("hello, " + s)
* eg: from cs50 import get_int

age = get_int("What's your age?\n")
print(f"You are at least {age * 365} days old.")
* eg: from cs50 import get_int

x = get_int("x: ")
y = get_int("y: ")

if x < y:
    print("x is less than y")
elif x > y:
    print("x is greater than y")
else:
    print("x is equal to y")
* eg: from cs50 import get_string

s = get_string("Do you agree?\n")

if s == "Y" or s == "y":
    print("Agreed.")
elif s == "N" or s == "n":
    print("Not agreed.")
* eg: for i in range(3):
    cough()

def cough():
    print("cough")
* eg: with main -> shows NameError: name cough is not defined.
def main():
    for i in range(3):
        cough()

def cough():
    print("cough")

main()
* Fixes th above error:
def main():
    cough(3)

def cough(n):
    for i in range(n):
        print("cough")

main()
* positive integer funcion:
from cs50 import get_int

def main():
    i = get_positive_int()
    print(i)

def get_positive_int():
    while True:
        n = get_int("Positive Integer: ")
        if n > 0:
            break
    return n

main()
* print ? in row:
for i in range(4):
    print("?", end="")
print()
* print # in column:
for i in range(3):
    print("#")
 => And without a loop: print("#\n" * 3, end="").
* nested loops:
for i in range(3):
    for j in range(3):
        print("#", end="")
    print()
 * In python integer overflow does not happen:
 from time import sleep

i = 1
while True:
    print(i)
    sleep(1)
    i *= 2
* This will continue until the integer can no longer fit in your computer’s memory.
* Floating-point imprecision, too, can be prevented by libraries that can represent decimal numbers with as many bits as are needed.
* list eg:
scores = []
scores.append(72)
scores.append(73)
scores.append(33)

print(f"Average: {sum(scores) / len(scores)}")
* Iterate over each char in string:
from cs50 import get_string

s = get_string("Input:  ")
print("Output: ", end="")
for c in s:
    print(c, end="")
print()
# More features
* command-line arguments eg:
from sys import argv

for i in range(len(argv)):
    print(argv[i])
 * command line arguments other way:
 from sys import argv

for arg in argv:
    print(arg)
 * exit code when program exit eg:
 from sys import argv, exit

if len(argv) != 2:
    print("missing command-line argument")
    exit(1)
print(f"hello, {argv[1]}")
exit(0)
* linear search eg: 
import sys

names = ["EMMA", "RODRIGO", "BRIAN", "DAVID"]

if "EMMA" in names:
    print("Found")
    sys.exit(0)
print("Not found")
sys.exit(1)
* dictionary key value pairs:
import sys

people = {
    "EMMA": "617-555-0100",
    "RODRIGO": "617-555-0101",
    "BRIAN": "617-555-0102",
    "DAVID": "617-555-0103"
}

if "EMMA" in people:
    print(f"Found {people['EMMA']}")
    sys.exit(0)
print("Not found")
sys.exit(1)
* strings can be directly compared:
from cs50 import get_string

s = get_string("s: ")
t = get_string("t: ")

if s == t:
    print("Same")
else:
    print("Different")
* copying strings :
from cs50 import get_string

s = get_string("s: ")

t = s

t = t.capitalize()

print(f"s: {s}")
print(f"t: {t}")
* swap numbers:
x = 1
y = 2

print(f"x is {x}, y is {y}")
x, y = y, x
print(f"x is {x}, y is {y}")
# Files
* import csv
from cs50 import get_string

file = open("phonebook.csv", "a")

name = get_string("Name: ")
number = get_string("Number: ")

writer = csv.writer(file)
writer.writerow((name, number))

file.close()
* with open("phonebook.csv", "a") as file:
    writer = csv.writer(file)
    writer.writerow((name, number)) 
# New features
* A feature of Python that C does not have is regular expressions, or patterns against which we can match strings. For example, its syntax includes:
., for any character
.*, for 0 or more characters
.+, for 1 or more characters
?, for something optional
^, for start of input
$, for end of input
For example, we can match strings with:
import re
from cs50 import get_string

s = get_string("Do you agree?\n")

if re.search("^y(es)?$", s, re.IGNORECASE):
    print("Agreed.")
elif re.search("^no?$", s, re.IGNORECASE):
    print("Not agreed.")
