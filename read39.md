# Reading 2
## Reading and Writing Files in Python
This guide givess an overview about how to read/write a file using python. 

* def file: is where data is stored, mainly has three parts:Header, Data and end of file.
File paths: string represnts te location of the file,mainly has three parts:Folder Path, File Name, and Extention. 

Line ending is problem when indicating new line.

* Character Encodings
Another problem while encoding of the byte data. 
error happens when misrepresentation of the character in coding.

* Opening and Closing a File in Python: 
* to open a file => file = open('file_name.txt')
* to close a file => file.close 

* as in the article here the most common used modes: 
* 'r'	Open for reading (default)
* 'w'	Open for writing, truncating (overwriting) the file first
* 'rb' or 'wb'	Open in binary mode (read/write using byte data)
 
file objexts are mainly three categories : 
Text file:
open('file_name.txt.txt')
open('file_name.txt.txt', 'r')
open('file_name.txt.txt', 'w')
Buffered binary files: 
open('file_name.txt.txt', 'rb')
open('file_name.txt.txt', 'wb')
Raw binary files:
open('file_name.txt.txt', 'rb',buffering=0)

# Reading and Writing Opened Files:
reading a file(as per author): 
.read(size=-1)	This reads from the file based on the number of size bytes. If no argument is passed or None or -1 is passed, then the entire file is read.
.readline(size=-1)	This reads at most size number of characters from the line. This continues to the end of the line and then wraps back around. If no argument is passed or None or -1 is passed, then the entire line (or rest of the line) is read.
.readlines()	This reads the remaining lines from the file object and returns them as a list.

## writing files(as per author): 
.write(string)	This writes the string to the file.
.writelines(seq)	This writes the sequence to the file. No line endings are appended to each sequence item. It’s up to you to add the appropriate line ending(s).

## Working With Bytes: 

## Tips and Tricks: 
__file__=> excucte scripts and print thier status.
Appending to a File=> using 'a'charcter, can help in appening or start writing at the end of your file.
Working With Two Files at the Same Time:
reading from one file and writing into another one, then its possible.
Creating Your Own Context Manager: 
using the with statement along with __enter__ and __exit__., you’ll have a context manager.

the article at the end mentioned great articles for reading and writing CSV and JSON files, also some build-in libraries that can help. 
this you can find =>https://realpython.com/read-write-files-python/

# Python Exceptions: An Introduction: 
This article is more or less about handling exception swhen error occurs.
Syntax errors occur when the parser detects an incorrect statement.
ZeroDivisionError was the example shown, its an exception error.

## Raising an Exception: 
You can raise it when condition occurs.
by adding  raise Exception (".....") after your condition.

## The AssertionError Exception: 
You can use prior to the code crashing, if your condition is is Fasle then you can throw an The AssertionError Exception.

## The try and except Block: Handling Exceptions:
try is your normal part of the program.
except is the program’s response to any exceptions.

one of the examples (as per the article) was shown is:
try:
    linux_interaction()
    with open('file.log') as file:
        read_data = file.read()
except FileNotFoundError as fnf_error:
    print(fnf_error)
except AssertionError as error:
    print(error)
    print('Linux linux_interaction() function was not executed')
## The else Clause: 
## the else clause will be executed when no exceptions occurs.
## Cleaning Up After Using finally: 
this code is always running whether you encounterd an exception in try/else.
