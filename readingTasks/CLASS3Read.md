
# Java Basic:

### Explain the difference between an “int” and an “Integer” in Java.
In Java, int and Integer are related but have distinct differences:

int is a primitive data type. It holds a simple integer value, and it's used to store numerical values without any additional properties or methods.
Integer is a class that wraps an int value in an object. It's part of the Java standard library (java.lang package) and provides additional methods and features not available with the int primitive.

### What is the default value for ints? Integers?
The default value for an int primitive is 0. If you declare an int variable without assigning a value to it, it will automatically be set to 0.
The default value for an Integer object is null. If you declare an Integer object variable without explicitly initializing it, it will have a value of null.

### What is autoboxing? Unboxing?
Autoboxing: Autoboxing is the automatic conversion that Java performs between primitive types and their corresponding wrapper classes. For example, when you assign an int to an Integer, Java will automatically wrap the int value into an Integer object.


int primitiveInt = 42;
Integer boxedInt = primitiveInt; // Autoboxing
Unboxing: Unboxing is the reverse process of autoboxing. It involves automatically converting an object of a wrapper class back to its corresponding primitive value.


Integer boxedInt = 99;
int primitiveInt = boxedInt; // Unboxing

Autoboxing and unboxing make it easier to work with primitive types and their corresponding wrapper classes, as they allow you to seamlessly switch between the two representations without needing explicit conversions.


### List the three basic categories of exceptions.
- Checked Exceptions:
These are exceptions that are checked by the compiler at compile-time. You are required to handle or declare them using try-catch blocks or specifying them in the method's throws clause. Checked exceptions typically represent exceptional conditions that a well-written application might be able to recover from.

- Unchecked Exceptions (Runtime Exceptions):
These exceptions are not checked by the compiler during compile-time. They usually indicate programming errors, such as dividing by zero or accessing an array index that's out of bounds. Unlike checked exceptions, you're not required to handle or declare them explicitly, but you can if you want to.

- Errors:
Errors represent serious issues that usually cannot be handled by your application. They are often related to the environment in which your program is running, such as out-of-memory errors (OutOfMemoryError). Like unchecked exceptions, you're not required to handle or declare errors.

### What type of statement can you use to handle an exception?
To handle exceptions in Java, you use try-catch statements. The basic structure of a try-catch statement looks like this:



try {
    // Code that might throw an exception
} catch (ExceptionType1 e1) {
    // Code to handle ExceptionType1
} catch (ExceptionType2 e2) {
    // Code to handle ExceptionType2
} finally {
    // Code that will be executed regardless of whether an exception occurred or not
}

### Describe a situation where you think it would be useful to have a program that scans text.
. You can develop a Java program that uses the Scanner class to read through the log files and perform the following tasks:

Error Detection:
The program can scan the log files for specific error messages or patterns that indicate issues with the application. For instance, you might search for phrases like "error," "exception," or specific error codes.

Log Statistics:
The program can tally the occurrences of different events and provide statistics, such as the frequency of different error types, the most common error messages, and the distribution of events over time.

Alert Generation:
If critical errors are detected, the program can generate alerts or notifications for the operations team or developers, indicating that immediate action is required to address the identified issues.

### What is input from a Scanner broken down into?
In Java, when you use a Scanner to read input from a source (such as the console or a file), the input is broken down into smaller units called tokens. A token is a sequence of characters that represents a meaningful unit of data. The Scanner class uses specific delimiters (such as whitespace or custom delimiters) to determine where one token ends and the next one begins.