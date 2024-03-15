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








Answer: 

print("*****")
print("*    *")
print("*    *")
print("*    *")
print("*****")


for letter in name:
    print(letter, end=" ")
print()


if name == name[::-1]:
    print("The name is a palindrome.")
else:
    print("The name is not a palindrome.")

