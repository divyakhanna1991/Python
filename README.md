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
Ans:str="";    
for Row in range(0,7):    
    for Col in range(0,7):     
        if (Col == 1 or Col == 5 or (Row == 2 and (Col == 2 or Col == 4)) or (Row == 3 and Col == 3)):  
            str=str+"* "    
        else:      
            str=str+"  "    
    str=str+"\n"    
print(str);
b) Print your name by using for loop
Ans:name = "Hardik"
for letter in name:
    print(letter, end=' ')

c) check the user name is palindrome or not
Ans:def is_palindrome(username):
    username = username.lower()
    return username == username[::-1]
username = input("Enter a Name ")
if is_palindrome(username):
    print(f"{username} is a palindrome!")
else:
    print(f"{username} is not a palindrome.")
