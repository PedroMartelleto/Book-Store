# Book Store - Milestone 2 (Client)

Pedro Martelleto Bressane Rezende - 11795641

João Marcos Cardoso da Silva - 11795314

Antonio Luiz Carvalho Turano Filho - 10723919

## Requirements
 - General Requirements
    - The system must present to all users the list of books
    - When a book is selected by the user, a list of recommended books must be presented. The recommendations are based on a simple pre-calculated recommendation algorithm (this is the functionality specific to our application).
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
    - The system must store their name, id, phone, email and address.
    - The clients must be able to manage their payment methods (credit card or debit card)
    - The clients must be able to add, view and remove books in their cart
    - The clients must be able to buy books from the store
 - Requirements specific to Administrators
    - The system must store their name, id, phone and email
    - The system must contain a default administrator account, which starts with the username "admin" and the password "admin"
    - Only existing Administrators are allowed to create new Administrator accounts
    - Administrators must be able to add, update read and delete information relative to books in the database.


## Project Description

The goal of the project is to fulfill the [Requirements](#requirements) by developing an easy-to-use online store that uses the [Goodreads book database](https://www.kaggle.com/datasets/austinreese/goodreads-books) to present a catalog of books to the user. Several pages are presented in the website that implement the functionality described in the [Requirements](#requirements). A **Navigation Diagram** illustrating the interaction between those pages can be found [here](https://www.figma.com/file/xTA8quNUIcFnJdaKB3LAgx/Navigation-Diagram?node-id=0%3A1).

To prepare for the development of the frontend, we developed a **[Mockup](https://www.figma.com/file/ZpRNOgvVlgQQf5CxK1sVEg/Book-Store---Mockup?node-id=0%3A1)** that details the widgets present in each page and the Graphical User Interface presented to the end user. The mockup has all the pages that will be in the final app, with variants depending on the type of user logged in (Admin or Customer).

The basic funcionality includes two types of user: a Customer and a Administrator. The Customer is able to navigate the website looking for books to buy, add them to a Cart and buy those items using a Credit or Debit Card. The Administrator does not buy items. Instead, this type of account can edit the contents of existing items, remove items or create new items and add them to the store.


## Responsiveness

* All pages are fully responsive.

## Comments about the code

### Overall Organization

The code for the project is organized in the following way:

 - The code for the interactive and visual elements of the website is in the `client` folder.
 - The code for the server-side logic and the API endpoints is in the `server` folder. 

### About 'use strict'

Use strict is unnecessary inside ES6 modules, so it is omitted in the react application.
## Test Plan and Results

For the main webpage, we manually performed tests by interacting with the website in various different settings, such as navigating to different pages, adding items to the cart, buying items, registering a new user, logging in. When logged in as administrator, we also tested the ability to add, update and delete items and to remove users or make them administrators.

For the server-side application, use used the [Jest](https://jestjs.io/) testing framework to perform automatic tests that check that all API endpoints have the correct effects and, when necessary, only respond to requests that are correctly authenticated.

In the latest version of this project, all tests were executed with success.
## Build Procedures

Instructions for building and executing the client and server-side applications are provided in the README.md files inside their respective folders. Note that to fully test the client-side application, it is required that a server be running on the same machine.

For more details on running the client, refer to the [client folder README](https://github.com/PedroMartelleto/Book-Store/tree/main/Milestone%203%20-%20Fullstack/client).
For more information about running server, refer to the [server folder README](https://github.com/PedroMartelleto/Book-Store/tree/main/Milestone%203%20-%20Fullstack/server).

## Admin account

To test the admin account, use the following credentials:

```
admin@email.com
admin
```

## Problems and Comments

None.
