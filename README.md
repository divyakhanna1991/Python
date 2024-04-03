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



ANSWER CODE

def print_initial(name):
    for i in range(len(name)):
        if i == 0:
            print("*      *")
        elif i == len(name) // 2:
            print("*" + " " * (len(name) - 1) + "*")
        else:
            print("*")

def print_name(name):
    for i in range(len(name) + 2):
        print("*", end="")
    print()
    print("*" + name + "*")
    for i in range(len(name) + 2):
        print("*", end="")
    print()

def is_palindrome(name):
    return name == name[::-1]

name = "Pratham"
print_initial(name)
print_name(name)

user_name = input("Enter a name: ")
if is_palindrome(user_name):
    print(f"{user_name} is a palindrome!")
else:
    print(f"{user_name} is not a palindrome.")
