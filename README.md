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

Ans (a) :- for i in range(7):
    for j in range(7):
        if j == 0 or j == 6 or (i == j and j < 4) or (i + j == 6 and j > 3):
            print("*", end=" ")
        else:
            print(" ", end=" ")
    print()
    
Ans (b) :-
name = "Mohit"
for letter in name:
    print(letter, end=' ')

Ans (c) :-
def is_palindrome(username):
    username = username.lower()
    return username == username[::-1]
username = input("Enter a Name ")
if is_palindrome(username):
    print(f"{username} is a palindrome!")
else:
    print(f"{username} is not a palindrome.")
