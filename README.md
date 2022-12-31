# r-memory-management-simulation-in
# @author Eliyahu yishaiovizh

  
memory management simulation

#Description 

In this exercise we would like to build simulate how disk management works.
We will exercise 3 classes. 
Class 1 - called FsFile which is a class that keeps basic
 information about a file such as where the blocks that belong to that file are kept.
Class 2 - named FileDecriptor this class stores a pointer to FsFile and the name of the file.
Class 3 - called FsDisk, this is a department that manages the disk. In this department, 
we will save all the operations we do on the disk. Actually all management of the disk goes through this department.
In FsDisk have Vector called MainDir that save all file that exist in folder.
And Map that called OpenFileDescriptor that save the dile that opened.
In the FsDisk department, 7 functions were built:
#1 ListAll - print the disk.
#2 FsFormat - do format to all the disk and do free to allocaded.
#3 CreateFile - create file and ave in OpenFileDecriptor and save in MainDir. and return fd
#4 OpenFile -  openFile and add to Map OpenFileDecriptor.
#5 CloseFille - close file and delete file from Map FileDecriptor.
#6 WriteToFile - writh to file a string.
# 7 ReadfromFile  - read from file to a string. and return a string
#8 DelFile - delete file from MainDir. 
if typed 0 the function to do exit and free to object of disk.

# input 
the program accept number from 0 to 8 . 
all number will active function of the class of FsDisk.
Below is a table where you will know for each function what is the input for it:
#1 no input
#2 number of bloke size.
#3 a string of file.
#4 a string of file name.
#5 int of the fd
#6  int of fd , a string , and size of the string
# 7 int of fd , a string , and size of the num chars tou want to read.
#8   a string of file name


#output

 the program wil print the result of what you typed.
Below is what you will get if you typed a number between 0 and 8:
#1 print the disk.
#2 function of void.
#3 return fd of the file.
#4 return 1 or -1.
#5 return the fd or -1
#6  return -1 or 1.
# 7 return a string.
#8  return 1 or -1. 

#how to compile?
Compile:  g++ code_stub.cpp  -o code_stu
run : ./code_stu
