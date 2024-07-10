# Intro to Server side concerns with JavaScript
01. What do the letters of the acronym `CRUD` stand for?

  > Create, Read, Update, Delete

02. Each action that `CRUD` represents maps to an HTTP request. What HTTP request does each `CRUD` action correspond to?

  > Create (POST), Read (GET), Update (PUT), Delete (DELETE)

03. What does `ORM` stand for? Which `ORM` do we use when interacting with MongoDB

  > The Object-Relational Mappers we have used when interacting with MongoDB is Mongoose. 

04. Which two `HTTP` request types include a body?

  > PUT and POST

05. In a/an _______ coding model, when you call a function, it returns only when the action has finished and stops your program for the time the action takes. Likewise in a/an _______ coding model, multiple things are allowed to happen at one time. When you perform an action, your program continues to run.  Fill in the blanks.

  > Synchronous / Asynchronous

06. What are the three types of data relationships? Provide an example of each.

  > One-to-many: One owner listing many different car listing on GregsList. 
    Many-to-many: An example could be an order and a product. An order can have multiple products, price, etc... and a product can have multiple attributes like unit price, name, etc...
    One-to-one: An example could be a user account to a customer's profile where there can only be one user for a customer's profile and vice versa. 

07. What is middleware?

  > Middleware is software that different applications use to communicate with each other.

08. The ______ pipeline delivers information from the client while the ______ pipeline returns it. Fill in the blanks. 

  > Continuous integration / Continuous delivery

09. Demonstrate the pattern that is used to include a request query with the client's `HTTP` request providing the property `tag` and the value `winter`.

  > https//example.com/api/?tag=winter

10. What is a ***virtual property***?

  > A virtual property is a small javascript function that can be used to create properties based on values stored in an element or in the elements in its neighborhood.
