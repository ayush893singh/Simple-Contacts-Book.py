# Simple-Contacts-Book.py
contacts = {}

while True:
    choice = input("\n1-Add\n2-Search\n3-Exit :- ")
    
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
        break
        
    else:
        print("Invalid!\n")
