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
b) Print your name by using for loop

c) check the user name is palindrome or not


i=0

j=6

for row in range (4):

    for col in range(7):

        if row==col:

            print("*",end="")

        elif row==i and col==j:

            print("*",end="")

            i=i+1

            j=j-1

        else:

            print(end="")

    print()

print()

string="Varisha"

for letter in string:

    print(letter,end="")

print()

if string==reversed(string):

    print("Palindrome")

else:

    print("Not Palindrome")
