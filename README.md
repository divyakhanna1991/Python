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



ANSWER-

result_str = ""


for row in range(0, 7):

    for column in range(0, 7):

        
        
        if (column == 1 or ((row == 0 or row == 6) and (column > 1 and column < 5)) or (column == 5 and row != 0 and row != 6)):
            result_str = result_str + ""  # Append '' to the 'result_str'
        else:
            result_str = result_str + " "  # Append space (' ') to the 'result_str'

    result_str = result_str + "\n"  # Add a newline character after each row in 'result_str'


print(result_str)

username = input("Enter the username: ")

s = username.lower() 
s = ''.join(char for char in s if char.isalnum())

if s == s[::-1]:
    print("The username is a palindrome.")
else:
    print("The username is not a palindrome.")
