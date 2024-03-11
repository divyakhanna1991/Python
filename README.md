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
# a) Print first letter of your name
name = "Peter"
first_letter = name[0]

print(f"a) First letter of the name {name}:\n")
print(" *      *")
print(" *             *")
print(" *              *")
print(" *      *")
print(" *")
print(" *")
print(" *")
print(" *")

# b) Print your name using a for loop
print("\nb) Printing name using a for loop:")
for letter in name:
    print(letter)

# c) Check if the user's name is palindrome or not
def is_palindrome(word):
    return word == word[::-1]

user_name = input("\nEnter your name: ")
if is_palindrome(user_name.lower()):
    print("c) Your name is a palindrome!")
else:
    print("c) Your name is not a palindrome.")
