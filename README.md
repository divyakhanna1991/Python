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
#a) write the first letter of your name.
print("Ansh 221097035")
for row in range(7):
    for col in range(5):
        if (col == 0 or col == 4) or ((row == 0 or row == 3) and (col > 0 and col < 4)):
            print("*", end="")
        else:
            print(end=" ")
    print()

        
            
        

# #b) print your name by using for loop.
name="Ansh"
for letters in name:
     print (letters)

#c) Check whether user name is palindrome or not.
def palindrome(word):
    x=word.replace(" ","")
    return x==x[::-1]

username = input("Enter your name:-")

if palindrome(username):
    print(f"{username} is a palindrome!")
else:
    print(f"{username} is not a palindrome.")
