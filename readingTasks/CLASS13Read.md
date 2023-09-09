# Class 13

## 1. Real-life examples of "One-to-Many" relationships:

In a "One-to-Many" relationship, one entity is associated with multiple instances of another entity. Here are a few real-life examples:

a. Author and Books: An author can write many books, but each book is written by only one author.

b. Teacher and Students: A teacher can have many students in a class, but each student has only one teacher for that class.

c. Parent and Children: A parent can have multiple children, but each child has only one set of parents.

d. Customer and Orders: A customer can place multiple orders, but each order is placed by one customer.

## 2. Creating a One-to-Many relationship between Player and Team:

In this scenario, if you want to create a one-to-many relationship between Player and Team, typically, a Player would be the "many" side, and Team would be the "one" side. This means that each player can be a part of only one team (one team can have many players), making Team the owning side of the relationship.

## 3. Explaining One-to-Many relationships to a non-technical friend:

Imagine you have a collection of boxes. Each box can contain multiple items, but each item belongs to only one box. This is similar to a one-to-many relationship. Each box represents the "one" side, and the items inside are the "many" side. So, a box (one) can have many items (many), but each item belongs to only one box.

## 4. Difference between a unit test and an integration test:

Unit Test: A unit test focuses on testing a small, isolated piece of code, typically a single function or method, in isolation from the rest of the application. It aims to ensure that the individual unit of code works correctly. Mocks and stubs are often used to isolate the unit being tested from external dependencies.

Integration Test: An integration test, on the other hand, tests the interaction between different components or modules of an application. It checks if these components work correctly when combined. Integration tests are used to verify that the different parts of the system can work together as intended.

## 5. Object that provides support for Spring MVC Testing:

In Spring, the primary object that provides support for Spring MVC testing is the MockMvc class, which is part of the Spring Test framework. It allows you to simulate HTTP requests and test the behavior of your controllers and the entire request-response cycle in a controlled and isolated environment without making actual HTTP calls.

## 6. What does the "perform()" method do in a Spring integration test:

In Spring integration testing using MockMvc, the perform() method is used to simulate an HTTP request and perform an action on a specified URL. It sends a request to your Spring MVC controller and allows you to specify parameters, headers, and other aspects of the request. You can use it to trigger controller actions (e.g., GET, POST) and then assert the response to ensure that your controller behaves as expected during testing. It's a key method for conducting integration tests on your Spring MVC controllers.