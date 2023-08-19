### Explain the difference between an object and a class.
Class:
A class in Java is a blueprint or template for creating objects. It defines the properties (also called attributes or fields) and behaviors (also called methods) that objects of that class will have. A class serves as a prototype for creating multiple instances (objects) that share the same structure and behavior. It encapsulates the data and functionality related to a specific concept.

Object:
An object is an instance of a class. It is a concrete, real-world representation of the class's blueprint. Objects have their own unique set of attributes (properties) and can execute the methods defined in their class. Objects are created from classes and are used to model and interact with real-world entities or concepts.

### Name two types of state that a Student object might have.
Name: The name of the student is an example of a state. It's a property that distinguishes one student object from another.

Age: The age of the student is another type of state. It represents a characteristic specific to each student object.

### Name two types of behaviours that a student object might have.
Enroll in Course: This behavior involves the student object interacting with the system to enroll in a specific course. It might involve updating the student's course list and other related data.

Calculate GPA: This behavior would involve the student object performing calculations to determine their grade point average (GPA) based on their coursework and grades. It might involve accessing the student's grades and performing mathematical operations.

### Explain the significance of a constructor for a class.
A constructor is a special method in Java that is used to initialize the newly created objects of a class. It is called automatically when an object is created using the new keyword. Constructors are used to set initial values for the attributes (fields) of an object and perform any necessary setup operations. Constructors ensure that objects are properly initialized before they are used, helping to avoid unexpected behavior and errors due to uninitialized state.

Key points about constructors:

Constructors have the same name as the class.
They don't have a return type, not even void.
If a class does not explicitly define any constructors, a default constructor (with no arguments) is provided by Java.

### Write the declaration statement for a class named “Student” (do not fill it with fields and methods).
Here's the declaration statement for a class named "Student" without filling it with fields and methods:


public class Student {
    // Fields and methods will be added here
}

### What is the value of the binary number 1101?
The binary number 1101 represents the decimal value 13.

### Write the number 52 in binary. Write it in hexidecimal.
 the binary representation of decimal 52 is 110100
the hexadecimal representation of decimal 52 is 0x34