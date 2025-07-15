# Core Java Interview Questions and Answers

## 1. Java Basics

**1. What is Java?**  
Java is a high-level, object-oriented, class-based programming language developed by Sun Microsystems (now Oracle).

**2. What are the features of Java?**  
- Platform-independent  
- Object-oriented  
- Secure  
- Robust  
- Multithreaded  
- Portable  
- Architecture-neutral

**3. What is JVM, JRE, and JDK?**  
- **JVM**: Java Virtual Machine (executes bytecode)  
- **JRE**: Java Runtime Environment (JVM + libraries)  
- **JDK**: Java Development Kit (JRE + development tools)

**4. What is the difference between JDK and JRE?**  
JDK is used for development, while JRE is used for running Java programs.

**5. Why is Java platform-independent?**  
Because Java programs are compiled into bytecode, which can be executed on any JVM.

---

## 2. Data Types, Variables, and Operators

**6. What are the data types in Java?**  
- **Primitive**: int, float, char, boolean, etc.  
- **Non-primitive**: String, Array, Class, Interface

**7. What is type casting?**  
Converting one data type to another.  
Example: `int a = (int) 10.5;`

**8. Difference between `==` and `.equals()`?**  
- `==` compares object references  
- `.equals()` compares values (can be overridden)

**9. What are wrapper classes?**  
Classes that wrap primitive types into objects (e.g., `int` → `Integer`).

**10. What is autoboxing and unboxing?**  
- **Autoboxing**: Automatic conversion from primitive to wrapper  
- **Unboxing**: Wrapper to primitive

---

## 3. OOPs Concepts

**11. What is Object-Oriented Programming (OOP)?**  
Programming model organized around objects rather than logic and functions.

**12. What are the 4 principles of OOP?**  
- Inheritance  
- Encapsulation  
- Polymorphism  
- Abstraction

**13. What is inheritance?**  
A class acquires the properties and methods of another class using `extends`.

**14. What is method overloading?**  
Same method name with different parameters in the same class.

**15. What is method overriding?**  
Same method in superclass and subclass, with different implementation.

**16. What is abstraction?**  
Hiding implementation details and showing only essential features.

**17. What is encapsulation?**  
Binding variables and methods together using classes.

**18. What is polymorphism?**  
Ability of an object to take many forms. (Compile-time and runtime)

**19. Difference between abstract class and interface?**  
- Abstract class: can have method body  
- Interface: only abstract methods (Java 7), default and static methods allowed (Java 8+)

**20. Can interfaces have static methods?**  
Yes, since Java 8.

---

## 4. Constructors and Initialization

**21. What is a constructor?**  
A special method to initialize objects, called when an object is created.

**22. Can constructors be overloaded?**  
Yes, multiple constructors can be defined with different parameters.

**23. What is a default constructor?**  
A no-argument constructor provided by the compiler if none is written.

**24. What is constructor chaining?**  
Calling one constructor from another using `this()` or `super()`.

---

## 5. Exception Handling

**25. What is an exception?**  
An unwanted event that interrupts normal program flow.

**26. Checked vs Unchecked Exceptions?**  
- **Checked**: Compile-time (e.g., IOException)  
- **Unchecked**: Runtime (e.g., NullPointerException)

**27. What is the finally block?**  
Used to execute code after try/catch, regardless of exception outcome.

**28. Can try block exist without catch or finally?**  
No, it must be followed by catch or finally block.

---

## 6. Strings and StringBuffer

**29. Difference between String, StringBuilder, and StringBuffer?**  
- **String**: Immutable  
- **StringBuilder**: Mutable, not thread-safe  
- **StringBuffer**: Mutable, thread-safe

**30. How are strings stored in memory?**  
In a String Constant Pool.

**31. Why are strings immutable in Java?**  
For security, thread-safety, and caching.

---

## 7. Arrays and Collections

**32. What is an array?**  
A container for fixed-size elements of the same type.

**33. What are the limitations of arrays?**  
Fixed size, can only store similar type data.

**34. What is Collection framework?**  
A set of classes and interfaces for storing and manipulating data.

**35. Differences: List vs Set vs Map?**  
- **List**: Ordered, allows duplicates  
- **Set**: Unordered, no duplicates  
- **Map**: Key-value pairs

**36. Difference between ArrayList and LinkedList?**

| Feature      | ArrayList       | LinkedList         |
|--------------|------------------|---------------------|
| Access Speed | Fast (index-based)| Slower (sequential) |
| Insert/Delete| Slow (shift elements)| Fast (link update) |

---

## 8. Multithreading

**37. What is a thread?**  
A thread is a lightweight subprocess for multitasking within a program.

**38. How to create a thread in Java?**  
- By extending `Thread` class  
- By implementing `Runnable` interface

**39. Difference between start() and run()?**  
- `start()`: Creates a new thread  
- `run()`: Runs on the current thread

**40. What is synchronization?**  
Controlling access to shared resources to prevent conflicts.

---

## 9. Keywords

**41. Use of `final` keyword?**  
- Variable: constant  
- Method: can't be overridden  
- Class: can't be extended

**42. Use of `static` keyword?**  
Belongs to the class instead of object.

**43. Difference between static and instance variables?**  
- Static: Shared across all instances  
- Instance: Separate for each object

---

## 10. Java Memory Management

**44. What is garbage collection?**  
Process of automatically deleting unused objects to free memory.

**45. What are strong, weak, and soft references?**  
- **Strong**: Not GC’d  
- **Weak**: GC’d at next cycle  
- **Soft**: GC’d only if memory is low

---

## 11. Java 8 Features

**46. What are lambda expressions?**  
Syntax for writing anonymous functions:  
```java
(param) -> expression
