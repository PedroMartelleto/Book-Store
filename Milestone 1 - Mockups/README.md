# Book Store - Milestone 1 (Mockups)

Pedro Martelleto Bressane Rezende - 11795641

João Marcos Cardoso da Silva - 11795314

Antonio Luiz Carvalho Turano Filho - 10723919

## Requirements
 - General Requirements
    - The system must present to all users the list of books
    - **When a book is selected by the user, a list of recommended books must be presented. The recommendations are based on a simple pre-calculated recommendation algorithm (this is the functionality specific to our application).**
    - The system must have two types of users, Clients and Administrators 
    - All types of user must be able to read and update the information associated with their account
    - All types of user must be able to delete their own account
    - The system must provide accessibility features
    - The system must have good usability
    - The system must be responsive
  - Requirements specific to Books
    - The list of all books must be stored in a database
    - The following information must be shown to the users:
      - Name
      - Photo
      - Description
      - Price
      - Rating (from 0 to 5 stars)
      - Author
      - Genre
      - Publication date
      - Page Count
    - Additionaly, the system must store the following information about each product:
      - The ID of the book
      - The quantity in stock
      - The number of times the book has been purchased
    - The system must also store all information necessary for the recommendation system.
  - Requirements specific to Clients
    - Anyone must be able to create a Client account
    - The system must store their first name, last name, email, password, address, zip, state, ZIP code and payment information
    - The clients must be able to manage their payment methods (credit card or debit card)
    - The clients must be able to add, view and remove books in their cart
    - The clients must be able to buy books from the store
 - Requirements specific to Administrators
    - The system must store their first name, last name, email, password, address, city, state and ZIP code
    - The system must contain a default administrator account, which starts with the username "admin" and the password "admin"
    - Only existing Administrators are allowed to create new Administrator accounts
    - Administrators must be able to add, update read and delete information relative to books in the database.

## Project Description

The goal of the project is to fulfill the [Requirements](#requirements) by developing an easy-to-use online store that uses the [Goodreads book database](https://www.kaggle.com/datasets/austinreese/goodreads-books) to present a catalog of books to the user. Several pages are presented in the website that implement the functionality described in the [Requirements](#requirements). A **Navigation Diagram** illustrating the interaction between those pages can be found [here](https://www.figma.com/file/xTA8quNUIcFnJdaKB3LAgx/Navigation-Diagram?node-id=0%3A1).

To prepare for the development of the frontend, we developed a **[Mockup](https://www.figma.com/file/ZpRNOgvVlgQQf5CxK1sVEg/Book-Store---Mockup?node-id=0%3A1)** that details the widgets present in each page and the Graphical User Interface presented to the end user. The mockup has all the pages that will be in the final app, with variants depending on the type of user logged in (Admin or Customer).

The basic funcionality includes two types of user: a Customer and a Administrator. The Customer is able to navigate the website looking for books to buy, add them to a Cart and buy those items using a Credit or Debit Card. The Administrator does not buy items. Instead, this type of account can edit the contents of existing items, remove items or create new items and add them to the store.

## HTML/CSS of the main pages

* See [Homepage.html](Homepage.html), [Products.html](Products.html) and [ProductDetail.html](ProductDetail.html). To test locally, also download the required resources contained in [BookStore_files/](BookStore_files).

## Responsiveness

* All pages are fully responsive.

## Comments about the code

None currently.

## Test Plan and Results

Does not apply.

## Build Procedures

Does not apply.

## Problems and Comments

None.
