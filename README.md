# PYTHON-PROJECT-
# Library Management System


library = []

def add_book():
    book = input("Enter Book Name: ")
    library.append(book)
    print("Book Added Successfully!")

def view_books():
    if len(library) == 0:
        print("No books available.")
    else:
        print("\nBooks in Library:")
        for book in library:
            print("-", book)

def search_book():
    book = input("Enter Book Name to Search: ")
    if book in library:
        print("Book Found!")
    else:
        print("Book Not Found!")

while True:
    print("\n===== Library Management System =====")
    print("1. Add Book")
    print("2. View Books")
    print("3. Search Book")
    print("4. Exit")

    choice = input("Enter your choice: ")

    if choice == "1":
        add_book()
    elif choice == "2":
        view_books()
    elif choice == "3":
        search_book()
    elif choice == "4":
        print("Thank you for using Library Management System!")
        break
    else:
        print("Invalid Choice! Try Again.")