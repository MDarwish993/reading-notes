# Reading Class 11

# Spring App Basics

## Role of `@Controller` classes in a Spring MVC application
`@Controller` classes in Spring MVC handle incoming web requests. They manage the flow of the application, processing requests, and returning appropriate responses. They often interact with services and repositories to gather data and render views.

## Explanation of a GET request for a non-technical friend
Imagine you're browsing the internet and you ask a website for a specific page. When you type a website's address into your browser and hit enter, you're sending a GET request. It's like asking for information, and the website sends back the page you requested.

## Annotation for Spring Boot application class
The annotation `@SpringBootApplication` should be placed on the main class of your Spring Boot application. It combines three annotations: `@Configuration`, `@EnableAutoConfiguration`, and `@ComponentScan`.

## Spring MVC and Thymeleaf

### Method for displaying Java variable in HTML using Thymeleaf
In a Spring Controller, you can use the `addAttribute()` method from the `Model` class to pass variables. These variables, known as model attributes, can then be accessed and displayed in HTML using Thymeleaf's expression language, typically by referencing them within HTML tags or attributes.

### Role of a `@Controller` class in a Spring MVC application
A `@Controller` class in Spring MVC is responsible for handling incoming HTTP requests. It processes these requests, performs necessary business logic, retrieves data from the model, and then selects a view to be rendered as a response. It acts as an entry point for various functionalities in the application.

### Definition of a model attribute in Thymeleaf
In Thymeleaf, a model attribute refers to the data objects passed from the controller to the view layer. These attributes contain data retrieved from the backend and are made accessible to the Thymeleaf templates for dynamic rendering. Thymeleaf expressions can then access and display these model attributes in HTML.

