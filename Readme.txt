Library Management System
Overview
This is a simple console-based Library Management System built in Java. It allows users to perform the following operations:

Add books to the library.
Borrow books.
Return borrowed books.
View available books in the library.
This application manages a collection of books, keeps track of their availability, and allows users to interact with the library via a text-based menu interface.

Features
Add books: Add new books to the library by providing a book title and author.
Borrow books: Borrow books from the library if they are available.
Return books: Return borrowed books to the library.
View available books: Display a list of books that are available for borrowing.
Input validation: Handles invalid inputs gracefully and provides feedback.
Technologies Used
Java: The core programming language.
In-memory data storage: Books are stored in an in-memory list (ArrayList).
CLI Interface: Text-based user interface implemented in Java.
Custom Exception Handling: For managing book borrowing/returning processes.
Requirements
Java 8 or later installed on your machine to compile and run the application.
Setup & Installation
1. Clone the Repository
Clone this repository to your local machine:

bash
Copy
git clone https://github.com/your-username/library-management-system.git
2. Compile the Code
Navigate to the project directory and compile the Java files:

bash
Copy
cd library-management-system
javac -d bin src/*.java
3. Run the Application
After compiling, you can run the program:

bash
Copy
java -cp bin LibraryApp
This will start the Library Management System, where you can interact with the application via the terminal.

Usage
Once the program is running, you'll see the following menu:

sql
Copy
Library System Menu:
1. Borrow a Book
2. Return a Book
3. View Available Books
4. Add a New Book
5. Exit
Please select an option:
Operations:
Borrow a Book: Enter the title of the book you wish to borrow. If the book is available, it will be marked as borrowed.
Return a Book: Enter the title of the book you wish to return. If the book is already borrowed, it will be marked as available again.
View Available Books: Displays a list of books that are currently available in the library.
Add a New Book: Add a new book by providing the title and author.
Exit: Exit the application.
Sample Interaction:
vbnet
Copy
Library System Menu:
1. Borrow a Book
2. Return a Book
3. View Available Books
4. Add a New Book
5. Exit
Please select an option: 3

Books in the library:
Java Programming by John Doe [Available]
Data Structures by Jane Smith [Available]
Design Patterns by Robert C. Martin [Available]

Library System Menu:
1. Borrow a Book
2. Return a Book
3. View Available Books
4. Add a New Book
5. Exit
Please select an option: 1

Enter book title to borrow: Java Programming
You have borrowed: Java Programming

Library System Menu:
1. Borrow a Book
2. Return a Book
3. View Available Books
4. Add a New Book
5. Exit
Please select an option: 3

Books in the library:
Data Structures by Jane Smith [Available]
Design Patterns by Robert C. Martin [Available]
Java Programming by John Doe [Borrowed]
Code Structure
Book.java: Represents the Book entity with attributes such as title, author, and availability status.
Library.java: Contains methods to manage the library's collection, such as adding books, borrowing books, and returning books.
LibraryApp.java: Main class that runs the application, interacting with the user and the library system.
UserInterface.java: Displays the menu and takes user input to navigate the application.
BookNotAvailableException.java (optional): Custom exception for managing errors related to borrowing unavailable books.
Enhancements (Optional)
Database Integration: Switch from in-memory storage to a database like SQLite to persist data.
User Authentication: Add user login functionality to track borrowing history per user.
Due Dates: Implement borrowing with due dates, allowing for overdue book tracking.
Graphical User Interface (GUI): Use JavaFX or Swing to create a GUI-based version of the library system.
Reports/Export: Use libraries like Apache POI for exporting book data or reports.