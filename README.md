Homework Assignment: Online Bookstore RESTful API

Objective:
Design and implement a RESTful API for an online bookstore using Java and Spring Boot. This
API should provide essential functionality for both the user and the bookstore admin.
Requirements:
1. Entities:
- Book: ISBN (unique identifier), Title, Author, Price, Stock Quantity, CreatedAt,
UpdatedAt.
- User: ID, Name, Email, Password (encrypted), CreatedAt, UpdatedAt.
- Order: Order ID, User ID, Total Price, List of Books, Order Date, CreatedAt,
UpdatedAt.
2. API Endpoints:
- Book:
- `GET /books`: Retrieve a list of all books ordered by creation date
DESC.
- `GET /books/{isbn}`: Retrieve details of a book by ISBN.
- `POST /books`: Add a new book (Admin only).
- `PUT /books/{isbn}`: Update details of a book (Admin only).
- `DELETE /books/{isbn}`: Delete a book by ISBN (Admin only).
- User:
- `POST /users/signup`: Register a new user.
- `POST /users/login`: Authenticate a user and return a token (JWT
preferred).

- Order:
- `POST /orders`: Place a new order for a user with a minimum price of
25$.
- `GET /orders/{userId}`: Get all orders for a specific user ordered by
update date DESC.
- `GET /orders/details/{orderId}`: Get details of a specific order by its ID
with the books under that order.

3. Features:
- Use Spring Boot's layered architecture: Controller, Service, DAO, Entity.
- Implement security: Passwords should be securely hashed, and only
authenticated users should be able to place orders. Admin operations (e.g.,
adding or deleting a book) should require admin privileges.
- Integrate a database of your choice (e.g., H2 for simplicity, MySQL, or
PostgreSQL for more realism) using Spring Data JPA.

- Include basic error handling (Book not found, Insufficient stock, Unauthorized
user, Minimum Price For Order).
4. Bonus:
- Implement pagination for the `GET /books` endpoint.
- Implement HATEOAS (Hypermedia as the Engine of Application State) to guide
the clients on possible interactions with your API.
- Implement Swagger UI integration.
- Add a simple rate-limiting mechanism to prevent abuse.
- Include unit and integration tests for your application using JUnit and MockMvc.
Submission:
Please submit your project as a GitHub repository. The solution should compile and run
without any errors. We will review the code quality, design patterns, and adherence to the
requirements.Homework Assignment: Online Bookstore RESTful API

Objective:
Design and implement a RESTful API for an online bookstore using Java and Spring Boot. This
API should provide essential functionality for both the user and the bookstore admin.
Requirements:
1. Entities:
- Book: ISBN (unique identifier), Title, Author, Price, Stock Quantity, CreatedAt,
UpdatedAt.
- User: ID, Name, Email, Password (encrypted), CreatedAt, UpdatedAt.
- Order: Order ID, User ID, Total Price, List of Books, Order Date, CreatedAt,
UpdatedAt.
2. API Endpoints:
- Book:
- `GET /books`: Retrieve a list of all books ordered by creation date
DESC.
- `GET /books/{isbn}`: Retrieve details of a book by ISBN.
- `POST /books`: Add a new book (Admin only).
- `PUT /books/{isbn}`: Update details of a book (Admin only).
- `DELETE /books/{isbn}`: Delete a book by ISBN (Admin only).
- User:
- `POST /users/signup`: Register a new user.
- `POST /users/login`: Authenticate a user and return a token (JWT
preferred).

- Order:
- `POST /orders`: Place a new order for a user with a minimum price of
25$.
- `GET /orders/{userId}`: Get all orders for a specific user ordered by
update date DESC.
- `GET /orders/details/{orderId}`: Get details of a specific order by its ID
with the books under that order.

3. Features:
- Use Spring Boot's layered architecture: Controller, Service, DAO, Entity.
- Implement security: Passwords should be securely hashed, and only
authenticated users should be able to place orders. Admin operations (e.g.,
adding or deleting a book) should require admin privileges.
- Integrate a database of your choice (e.g., H2 for simplicity, MySQL, or
PostgreSQL for more realism) using Spring Data JPA.

- Include basic error handling (Book not found, Insufficient stock, Unauthorized
user, Minimum Price For Order).
4. Bonus:
- Implement pagination for the `GET /books` endpoint.
- Implement HATEOAS (Hypermedia as the Engine of Application State) to guide
the clients on possible interactions with your API.
- Implement Swagger UI integration.
- Add a simple rate-limiting mechanism to prevent abuse.
- Include unit and integration tests for your application using JUnit and MockMvc.
Submission:
Please submit your project as a GitHub repository. The solution should compile and run
without any errors. We will review the code quality, design patterns, and adherence to the
requirements.
