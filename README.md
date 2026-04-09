## Contact Management System (Python CLI)
A simple and beginner-friendly Command Line Contact Management System built using Python. This application allows users to add and search contacts efficiently using a dictionary-based approach.

## Features
Add new contacts
Search existing contacts
Prevent duplicate phone numbers
Exit the application safely
Simple logic, easy to understand

## Technologies Used
Python 3
    Core Concepts:
    Dictionaries
    Loops (while)
    Conditional Statements (if-elif-else)
    User Input/Output

## How to Run
Run the following command in terminal:

## python contacts.py
## How It Works
The program uses a Python dictionary:
contacts = { "Name": "Phone Number" }
It continuously displays a menu:

1 - Add Contact
2 - Search Contact
3 - Exit
* Add Contact
User enters name and phone number
Program checks for duplicate numbers
Stores data in dictionary
* Search Contact
User enters name
Program returns phone number or "Not found"
 * Exit
Stops the program execution
## Code
```
contacts = {}

while True:
    choice = input("\n1-Add\n2-Search\n3-Exit \nEnter your Choice :- ")
    
    if choice == '1':
        name = input("\nName: ")
        phone = input("Phone Number: ")
    
        if phone in contacts.values():
            print("This phone number is already added!\n")
        else:
            contacts[name] = phone
            print("Added!\n")
        
    elif choice == '2':
        name = input("Name to search: ")
        print(contacts.get(name, "Not found"), "\n")
        
    elif choice == '3':
        print("Thank You!")
        break
        
    else:
        print("Invalid!\n")
```
## Output
```
1-Add
2-Search
3-Exit 
Enter your Choice :- 1

Name: Rahul
Phone Number: 9876543210
Added!

1-Add
2-Search
3-Exit 
Enter your Choice :- 2
Name to search: Rahul
9876543210

1-Add
2-Search
3-Exit 
Enter your Choice :- 3
Thank You!
```
## Author
Ayush Singh
GitHub: @ayush893singh
