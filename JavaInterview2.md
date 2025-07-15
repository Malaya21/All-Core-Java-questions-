# Core Java Interview Questions and Answers (Part 2)

---

## 13. Java Collections – Advanced

**56. What is the difference between Iterator and ListIterator?**  
- **Iterator**: Can traverse in forward direction.  
- **ListIterator**: Can traverse in both directions (forward/backward).

**57. Difference between ArrayList and Vector?**  
- **ArrayList**: Not synchronized, faster.  
- **Vector**: Synchronized, slower.

**58. What is the difference between Set and Map?**  
- **Set**: Collection of unique elements.  
- **Map**: Key-value pairs, keys must be unique.

**59. What is the difference between HashSet and TreeSet?**  
- **HashSet**: No order maintained, faster.  
- **TreeSet**: Sorted in natural order, slower.

**60. What is LinkedHashMap?**  
A HashMap that maintains insertion order.

**61. What is EnumSet?**  
A specialized Set implementation for use with enum types.

**62. What is Queue in Java?**  
A collection used to hold multiple elements prior to processing.

**63. What is PriorityQueue?**  
Queue where elements are ordered based on priority.

**64. What is a Deque?**  
Double-ended queue allowing insertion/removal from both ends.

**65. What are Comparable and Comparator interfaces?**  
- **Comparable**: Used to define natural ordering.  
- **Comparator**: Used for custom sorting.

---

## 14. Inner Classes

**66. What is an inner class?**  
A class defined within another class.

**67. Types of inner classes in Java?**  
- Member inner class  
- Static nested class  
- Local inner class  
- Anonymous inner class

**68. What is an anonymous class?**  
A class without a name, defined and instantiated in a single expression.

---

## 15. File I/O in Java

**69. What is the java.io package used for?**  
Provides classes for system input/output through data streams, serialization, and file system.

**70. Difference between FileReader and BufferedReader?**  
- **FileReader**: Reads character files.  
- **BufferedReader**: Buffers characters for efficient reading.

**71. How to write data to a file in Java?**  
Using `FileWriter` or `BufferedWriter`.

**72. What is serialization in Java?**  
Converting an object into a byte stream.

**73. What is Deserialization?**  
Reconstructing an object from a byte stream.

---

## 16. Java Annotations

**74. What are annotations?**  
Metadata about the code that provide information to the compiler or runtime.

**75. Common built-in annotations in Java?**  
- `@Override`  
- `@Deprecated`  
- `@SuppressWarnings`

**76. Can we create custom annotations in Java?**  
Yes, using `@interface`.

---

## 17. Java Reflection API

**77. What is the Reflection API?**  
Allows inspection and modification of classes, methods, and fields at runtime.

**78. Use cases for Reflection?**  
- Framework development  
- Serialization libraries  
- Testing tools

---

## 18. Java Memory & Garbage Collection

**79. What is the heap and stack in Java memory?**  
- **Heap**: Stores objects  
- **Stack**: Stores method calls and local variables

**80. What are memory leaks in Java?**  
Objects not properly garbage collected due to lingering references.

**81. Can we force garbage collection?**  
No, we can only request it using `System.gc()`.

**82. What are weak references used for?**  
To allow GC when an object is not strongly reachable.

---

## 19. Java Synchronization and Concurrency

**83. What is thread safety?**  
Code that functions correctly when accessed by multiple threads.

**84. What are synchronized blocks?**  
Used to lock an object so that only one thread can execute a block of code.

**85. Difference between wait() and sleep()?**  
- `wait()`: Releases the lock, waits until notified.  
- `sleep()`: Holds the lock, sleeps for a time.

**86. What is a deadlock?**  
Two or more threads waiting indefinitely for each other to release resources.

**87. How to avoid deadlock?**  
- Lock ordering  
- Try-lock mechanism  
- Avoid nested locks

**88. What is ReentrantLock?**  
A lock implementation providing more control than `synchronized`.

**89. What is the use of `volatile` in concurrency?**  
Ensures visibility of changes to variables across threads.

---

## 20. Java Design Patterns (Basics)

**90. What is a design pattern?**  
Reusable solution to common software design problems.

**91. Types of design patterns?**  
- Creational  
- Structural  
- Behavioral

**92. What is Singleton pattern?**  
A class that allows only one instance.

**93. What is Factory pattern?**  
A method returns instances without exposing instantiation logic.

**94. What is the Observer pattern?**  
Object notifies other objects on state change.

**95. What is Builder pattern?**  
Separate the construction of a complex object from its representation.

---

## 21. Java 8+ Features

**96. What is Stream API?**  
Process collections in a functional style using map, filter, reduce.

**97. Difference between Intermediate and Terminal operations?**  
- Intermediate: map, filter (returns Stream)  
- Terminal: collect, forEach, reduce (ends the stream)

**98. What is method reference?**  
Shorthand for lambda expressions using `::`.

**99. What is a default method in interface?**  
A method with a body, introduced in Java 8.

**100. What is a static method in interface?**  
Static method defined in interface (accessible via interface name).

---

## 22. Java 9–17 Key Additions (Brief)

**101. What is JShell?**  
A REPL (Read Evaluate Print Loop) tool introduced in Java 9.

**102. What are modules in Java 9?**  
Encapsulation and modularization of code using `module-info.java`.

**103. What are var keyword (Java 10)?**  
Local variable type inference.

**104. What is the new switch expression (Java 14)?**  
Allows switch to return values.

---

## 23. Java Best Practices

**105. Why use interfaces over abstract classes?**  
For multiple inheritance and API contracts.

**106. Why prefer composition over inheritance?**  
More flexible, avoids tight coupling.

**107. What is defensive copying?**  
Creating copies of mutable objects to prevent unintended changes.

**108. What is immutable class?**  
A class whose instances cannot be changed once created.

---

## 24. Miscellaneous Core Java Questions

**109. Difference between deep copy and shallow copy?**  
- **Shallow**: Copies references  
- **Deep**: Copies objects and their nested objects

**110. What is cloning in Java?**  
Creating an exact copy using `clone()`.

**111. What is marker interface?**  
An interface with no methods (e.g., `Serializable`, `Cloneable`).

**112. What is the difference between == and equals for String?**  
- `==`: Checks reference  
- `.equals()`: Checks value

**113. Why is String immutable?**  
For security, caching, and performance.

**114. What is class loader?**  
Part of JVM that loads classes during runtime.

**115. What is JavaBean?**  
A class with private properties, public getters/setters, and no-arg constructor.

**116. What is `instanceof` operator?**  
Checks if an object is an instance of a specific class/interface.

**117. What is the use of assert keyword?**  
Used for debugging, checking assumptions in code.

**118. Can you override a static method?**  
No, static methods are bound at compile time.

**119. Can we override a private method?**  
No, private methods are not inherited.

**120. What is the diamond problem and how does Java handle it?**  
Occurs with multiple inheritance. Java uses interfaces and avoids multiple class inheritance.

---

## 25. Common Coding Interview Patterns

**121. Reverse a String in Java?**  
```java
new StringBuilder(input).reverse().toString();
