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








str="D";    
for Row in range(0,7):    
    for Col in range(0,7):     
        if (Col == 1 or ((Row == 0 or Row == 6) and (Col > 1 and Col < 5)) or (Col == 5 and Row != 0 and Row != 6)):  
            str=str+"*"    
        else:      
            str=str+" "    
    str=str+"\n"    
print(str);

for i in "Dipak":
    print (i);
    
    
   

username = input("Enter the username: ")

s = username.lower() 
s = ''.join(char for char in s if char.isalnum())

if s == s[::-1]:
    print("The username is a palindrome.")
else:
    print("The username is not a palindrome.")












