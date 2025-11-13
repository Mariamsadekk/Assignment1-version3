
## Programming III – Assignment 01: Library Management System
**General Description**

In this project, you are tasked with implementing a Library Management System as a console application.
The system simulates different types of books, the library that holds them, and members who borrow them.
This milestone focuses on Object-Oriented Programming (OOP) concepts such as inheritance, encapsulation, and dynamic memory allocation.
The goal is to design the system’s structure in preparation for additional functionalities (borrowing history, fines, and due dates) in Milestone 2.

**Milestone 01: Required Classes and Methods**

**a) Book Class**

Represents a generic book in the library.
This class will serve as the base class for specific book types.

Attributes (all private):

- `string title`
- `int publicationYear`
- `bool isAvailable`

Methods:

- `void display()`: Displays the book’s title, year, and availability status.

- `void borrowBook()`: Marks the book as borrowed.

- `void returnBook()`: Marks the book as available again.

**Subclasses of Book**

- **Novel class** that has attribute:
  `string genre` (e.g., “Romance”, “Mystery”, etc.)
  
- **Magazine class** that has attribute:
  `int issueNumber`
  
- **Textbook class** that has attribute:
  `string subject`

**b) Library Class**

Represents a library that stores multiple books.

Attributes (all private):

- `Book* books` (dynamic array of book objects)
- `int capacity`
- `int currentCount`

Methods:

- `void addBook(const Book& b)`: Adds a book to the collection.

- `void displayBooks()`: Displays all books in the library.

**c) Member Class**

Represents a library member.

Attributes (all private):

- `string memberName`
- `int borrowedBooksCount`

Methods:

- `void displayInfo()`: Displays member details.

**d) Source File (main.cpp)**

Should consist of:

- A `main()` function that:

- Creates a Library object.
- Creates and adds 3 different book types (Novel, Magazine, Textbook) dynamically to the library.
- Creates a Member object with their details.
- Displays all library and member information using the **exact** console format below.

**🧾 Console Output**

Library Books:

Novel: The Silent Patient (Year: 2019, Genre: Thriller, Available)

Magazine: National Geographic (Year: 2023, Issue: 45, Available)

Textbook: Introduction to AI (Year: 2021, Subject: Computer Science, Borrowed)

Member Info:

Name: Omar Khaled

Borrowed Books: 1

**Important Notes**

- Cheating = 0 in the assignment.
- AI-generated code = 0 in the project.
- All attributes in classes must be private with setters/getters (if needed).
- Each class must have:

  - A default constructor
  - A parameterized constructor
  - A destructor (even if empty)


**Deliverables**

-A header file for each of the above classes.

-A single source file (.cpp) containing the main() function implementation.

-A text file including your name in the format:

**TutorialNumber_StudentID_StudentName**
e.g. T02_16002222_Ahmed Mohamed
