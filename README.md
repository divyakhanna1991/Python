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
(a)str="";    
j = 5;    
i = 0;  
for Row in range(0,7):    
    for Col in range(0,7):     
        if (Col == 1 or ((Row == Col + 1) and Col != 0)):  
            str=str+"*"    
        elif (Row == i and Col == j):  
              str=str+"*"    
              i=i+1  
              j=j-1  
        else:      
            str=str+" "    
    str=str+"\n"    
print(str);

c)def is_palindrome(username):
    username = username.lower()
    return username == username[::-1]
username = input("Enter a Name ")
if is_palindrome(username):
    print(f"{username} is a palindrome!")
else:
    print(f"{username} is not a palindrome.")
(b)name = "kartik"
for letter in name:
    print(letter, end=' ')
