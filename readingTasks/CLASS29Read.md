# Class 29

### What database engine is Room wrapped around? Do you think this is a good choice? Why or why not?

Room is wrapped around SQLite, which is a widely used and popular open-source relational database management system. Using SQLite as the underlying database engine for Room is generally a good choice for Android app development, and there are several reasons for this:

1. **Lightweight**: SQLite is a self-contained, serverless, and zero-configuration database engine, which makes it well-suited for mobile and embedded systems like Android. It has a small memory footprint and minimal setup requirements, which is important in resource-constrained environments.

2. **Proven Reliability**: SQLite has a long history of being stable and reliable. It's a mature database system with a well-established track record. Many well-known software projects, including Android, use SQLite.

3. **Compatibility**: SQLite databases are cross-platform, meaning that data created in an Android app can be easily transferred to other platforms or integrated with server-side databases. This makes it suitable for applications where data needs to be shared across different environments.

4. **Performance**: SQLite is known for its efficiency and performance, especially for common database operations found in mobile apps. It's optimized for reading and writing small to medium-sized datasets, which is typical in mobile applications.

5. **Integration with Android**: Room, as an Android-specific library, is tightly integrated with the Android framework. This integration simplifies database access and enhances the development experience, making SQLite a natural choice.

6. **Well-Supported**: SQLite is well-supported, with extensive documentation, a large user community, and frequent updates and improvements.

### Do Rooms have any similarities to JPA?
Yes, Room and JPA (Java Persistence API) share similarities in that they both provide object-relational mapping (ORM) capabilities, which allow developers to work with databases in an object-oriented way. However, there are also notable differences between them:

**Similarities:**

1. **Object-Relational Mapping (ORM):** Both Room and JPA are ORM frameworks. They allow you to define the structure of your database tables and relationships using object-oriented constructs, such as Java or Kotlin classes and annotations, rather than writing SQL queries directly.

2. **Annotations:** Both Room and JPA use annotations to map database tables to Java or Kotlin objects, specify relationships between entities, and define queries. Annotations make it easier to work with databases, as they generate SQL statements and handle the low-level database interactions behind the scenes.

3. **Abstraction:** Both Room and JPA provide an abstraction layer over the underlying database engine. This abstraction simplifies database interactions and allows developers to focus on working with objects instead of writing complex SQL code.

**Differences:**

1. **Platform:** Room is specifically designed for Android app development and integrates well with the Android ecosystem, whereas JPA is a Java EE (Enterprise Edition) technology primarily used in Java-based enterprise applications. This means that the choice between them depends on the platform you are developing for.

2. **Language:** JPA is typically used in Java applications, while Room is designed for Android apps, which can use Java or Kotlin. Room's support for Kotlin features is particularly strong, making it a preferred choice for Kotlin-based Android projects.

3. **Integration:** Room offers seamless integration with other Android components, such as LiveData and ViewModel, making it more suitable for Android development. It provides features that are tailored to Android-specific requirements, such as handling asynchronous data updates and lifecycle-aware components.

4. **Query Language:** While both Room and JPA support query annotations, they use different query languages. Room uses a subset of SQLite with its own annotations for defining queries, whereas JPA uses the JPQL (Java Persistence Query Language), which is similar to SQL but adapted for Java objects.


### Describe a DAO in your own words
A DAO, or Data Access Object, is a design pattern used in software development to abstract and centralize the access to a data source, typically a database, within an application. In essence, a DAO acts as an intermediary or interface between the application's business logic and the data source, shielding the rest of the application from the details of how data is stored, retrieved, and manipulated.

 DAO serves the following purposes:

1. **Abstraction**: It abstracts the underlying data source, allowing the application to work with data in an object-oriented manner, rather than dealing with raw database queries.

2. **Isolation**: It isolates the database-related code, making it easier to change the data source in the future without affecting the rest of the application.

3. **Clean Code**: It promotes cleaner, more maintainable code by centralizing data access logic.

4. **Testing**: It simplifies unit testing, as you can easily replace the actual DAO with mock objects during testing.

So, a DAO is like a bridge that connects your application to the database, shielding the application from the complexities of data storage and retrieval while providing a well-defined interface for working with data.