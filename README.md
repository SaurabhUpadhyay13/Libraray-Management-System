# Libraray-Management-System
Author-Saurabh Upadhyay
<br>
<br>
<br>

Welcome to the Library Management System project! This Python-based application, utilizing MySQL for database management and the Tkinter library for the graphical user interface, is designed to streamline the operations of a library. Whether you're managing a personal collection or overseeing a larger library, this system aims to provide an efficient and user-friendly solution.
<br>
<br>
Key Features
<br>
Add Book: Easily add new books to the library database with the click of a button.
<br>
Add Member: Keep track of library members by adding their information to the system.
<br>
Return Book: Manage book returns efficiently through a dedicated button.
<br>
Give Book: Facilitate the process of lending books to members.
<br>
Search Bar: Utilize the search bar to quickly find specific books within the library.
<br>
List Book: Choose from various options, such as viewing all books, borrowed books, or available books.
<br>
Statistics: Gain insights into the library's performance with a dedicated statistics feature.
<br>
<br>
Technologies Used
<br>
Python: The core programming language for the application's logic and functionality.
<br>
MySQL: A relational database management system used to store and manage book and member information.
<br>
Tkinter: A Python library for creating interactive and visually appealing graphical user interfaces.
<br>
<br>
<br>
1. Books Table:
<br>
Purpose: This table is designed to store information about the books available in the library.
<br>
Fields:
<br>
book_id (Primary Key): Unique identifier for each book.
<br>
title: Title of the book.
<br>
author: Author of the book.
<br>
language: langauge in which the book is available in library.
<br>
book_status: Indicates whether the book is available for borrowing.
<br>
![Book Table Screenshot](Screenshot 2024-01-01 191542.png)


<br>
Why Create It: The Books table is essential for maintaining a comprehensive catalog of all available books in the library, along with their key details.
<br>
<br>
2. Members Table:
<br>
<br>
Purpose: This table stores information about the members or patrons of the library.
<br>
Fields:
<br>
member_id (Primary Key): Unique identifier for each member.
<br>
member_name: Name of the member.
<br>
phone: Phone number of the member.
<br>
<br>
Why Create It: The Members table helps in managing and tracking the information of individuals who are registered library members, facilitating efficient communication and record-keeping.
<br>
<br>
3. Borrows Table:
<br>
<br>
Purpose: This table is responsible for recording instances when a member borrows a book from the library.
<br>
Fields:
<br>
borrow_id (Primary Key): Unique identifier for each borrowing transaction.
<br>
bmember_id (Foreign Key): Links to the Members table, indicating which member borrowed the book.
<br>
bbook_id (Foreign Key): Links to the Books table, indicating which book was borrowed.
<br>
<br>
Why Create It: The Borrows table helps in tracking the borrowing history of members, allowing the library to monitor book availability and manage due dates effectively.
<br>
<br>
4. Returns Table:
<br>
<br>
Purpose: This table records instances when a member returns a borrowed book.
<br>
Fields:
<br>
return_id (Primary Key): Unique identifier for each return transaction.
<br>
rborrow_id (Foreign Key): Links to the Borrows table, indicating the original borrowing transaction.
<br>
rmember_id: indicating the original borrowing member_id.
<br>
return_date: Date when the book was returned
<br>
<br>
Why Create It: The Returns table complements the Borrows table, providing a log of returned books. It helps in calculating any overdue fines, updating book availability, and maintaining accurate records of the library's collection.
<br>
<br>
