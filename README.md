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
Answer : 


str="";    
for Row in range(0,7):    
    for Col in range(0,7):     
        if (Col == 1 or ((Row == 0 or Row == 3) and Col > 1 and Col < 5) or (Col == 5 and Row != 0 and Row < 3) or (Col == Row - 1 and Row > 2)):  
            str=str+"*"    
        else:      
            str=str+" "    
    str=str+"\n"    
print(str);    

username = input("Enter the username: ")

s = username.lower() 
s = ''.join(char for char in s if char.isalnum())

if s == s[::-1]:
    print("The username is a palindrome.")
else:
    print("The username is not a palindrome.")


Answer :-

import re

aadhaar_details = {
    "123456789012": {"name": "Riya", "company": "ABC Corporation"},
    "234567890123": {"name": "Simran", "company": "XYZ Enterprises"}
}

def validate_aadhaar(aadhaar_number):
    if re.match(r"^\d{12}$", aadhaar_number):
        if aadhaar_number in aadhaar_details:
            return True
    return False

def display_aadhaar_details(aadhaar_number):
    if validate_aadhaar(aadhaar_number):
        details = aadhaar_details[aadhaar_number]
        print("Name:", details["name"])
        print("Company:", details["company"])
    else:
        print("Invalid Aadhaar number or details not found")

aadhaar_number = input("Enter Aadhaar number: ")
display_aadhaar_details(aadhaar_number)
2)
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
even_numbers = [num for num in numbers if num % 2 == 0]
even_indices_even_numbers = [numbers[i] for i in range(len(numbers)) if i % 2 == 0 and numbers[i] % 2 == 0]
occurrences = {num: numbers.count(num) for num in set(numbers)}

print("Even numbers:", even_numbers)
print("Even numbers from elements at even indices:", even_indices_even_numbers)
print("Occurrences of individual elements:", occurrences)
3)
class ShoppingCart:
    def init(self):
        self.cart = {}

    def add_item(self, item, price):
        if item in self.cart:
            self.cart[item] += price
        else:
            self.cart[item] = price

    def view_cart(self):
        if self.cart:
            print("Items in Cart:")
            for item, price in self.cart.items():
                print(item, ":", price)
        else:
            print("Cart is empty")

    def calculate_total(self):
        total = sum(self.cart.values())
        print("Total Price:", total)

cart = ShoppingCart()

while True:
    print("\n1. Add item to cart")
    print("2. View cart")
    print("3. Calculate total")
    print("4. Exit")

    choice = input("Enter your choice: ")

    if choice == '1':
        item = input("Enter item name: ")
        price = float(input("Enter item price: "))
        cart.add_item(item, price)
    elif choice == '2':
        cart.view_cart()
    elif choice == '3':
        cart.calculate_total()
    elif choice == '4':
        print("Exiting program...")
        break
    else:
        print("Invalid choice")
\]
Footer
