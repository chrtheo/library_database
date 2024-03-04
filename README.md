Library Database Design (Part of Advanced Databases Coursework)


Overview

The specific project is part of the Advanced Databases course in the MSc in Data Science that I attend. It is a basic library database which is intended to support a library in managing its collection, including books, authors, users, and loan transactions.


Database Requirements

The library system aims to document various entities such as books, their authors, users, and the details of each loan transaction. Below is a detailed description of the business rules governing this database:

•	Books: The database will catalog the library's extensive collection of books. Essential attributes to be recorded for each book include ISBN, title, the primary author (excluding co-authors for simplicity), genre, edition, page count, publication date, and price.

•	Authors: Each book is associated with a primary author. The database will assign a unique ID to each author and record details like last name, first name, birth and death dates (if applicable), country of origin, and gender.

•	Book Copies: While a book can have multiple copies within the library, each copy is linked to a single book title and possesses a unique ID. The only additional information required for a copy is its ISBN and the date it was purchased.

•	Loans: The system allows for the lending of book copies, with the stipulation that each loan pertains to a single copy. Each loan transaction is identified by a unique ID and includes details such as the user’s ID, loan date, and return date.

•	Users: User information is stored only if they have borrowed a book from the library. While a user may have multiple loans, each loan is specifically tied to a user. The database captures user details like last name, first name, email, contact information, and gender.


Implementation Guidelines

The creation of the database involves establishing a structured schema that accurately reflects the relationships between books, authors, copies, loans, and users as described. It is important to note the simplifications made for the purposes of this coursework, such as documenting only the primary author for each book and limiting loans to one copy per transaction, to streamline the database design process.


