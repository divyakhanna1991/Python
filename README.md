# Python
Programming in Python
Write python program to print first letter of your name 
a) Example: Peter
               *      *
               *             *
               *              *
               *      *
               *
               *
               *

Code

name = "Smarth"
rows = 7
for i in range(rows):
    for j in range(rows):
        if (i == 0 or i == rows//2 or i == rows-1) and (j > 0 and j < rows-1):
            print("*", end="")
        elif (j == 0 and i < rows//2) or (j == rows-1 and i > rows//2):
            print("*", end="")
        else:
            print(end=" ")

            
b) Print your name by using for loop


Code

name = "Smarth"
for letter in name:
    print(letter)

    
c) check the user name is palindrome or not

Code

name = "Smarth"
if name.lower() == name[::-1].lower():
    print("The name is a palindrome")
else:
    print("The name is not a palindrome")
