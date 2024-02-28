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


ANSWE:-
str="";    
for Row in range(0,7):    
    for Col in range(0,7):     
        if (Col == 1 or ((Row == 0 or Row == 3) and Col > 0 and Col < 5) or ((Col == 5 or Col == 1) and (Row == 1 or Row == 2))):  
            str=str+"*"    
        else:      
            str=str+" "    
    str=str+"\n"    
print(str);
print("b)")
for letter in name:
    print(letter, end=" ")
print()


palindrome = True
for i in range(len(name) // 2):
    if name[i] != name[-i - 1]:
        palindrome = False
        break

if palindrome:
    print("c) The name is a palindrome.")
else:
    print("c) The name is not a palindrome.")
