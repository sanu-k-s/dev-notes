Certainly! Here are 20 common Java interview questions and answers, along with examples where applicable:

1. **What is Java?**
   - **Answer:** Java is a high-level, platform-independent, and object-oriented programming language.

2. **What is the difference between JDK, JRE, and JVM?**
   - **Answer:** JDK (Java Development Kit) is for development, JRE (Java Runtime Environment) is for running Java applications, and JVM (Java Virtual Machine) executes Java bytecode.

3. **Explain the main features of Java.**
   - **Answer:** Java is known for its platform independence, object-oriented nature, automatic memory management (garbage collection), and strong type checking.

4. **What are the eight primitive data types in Java?**
   - **Answer:** byte, short, int, long, float, double, char, and boolean.

5. **What is the difference between `==` and `.equals()` for comparing objects in Java?**
   - **Answer:** `==` checks for reference equality, while `.equals()` is used to check for content equality.
   - **Example:**
     ```java
     String str1 = new String("Hello");
     String str2 = new String("Hello");
     boolean usingEquals = str1.equals(str2); // true
     boolean usingDoubleEquals = str1 == str2; // false
     ```

6. **What is the difference between `ArrayList` and `LinkedList` in Java?**
   - **Answer:** `ArrayList` is backed by an array, while `LinkedList` is backed by a doubly-linked list. `ArrayList` is faster for random access, whereas `LinkedList` is faster for insertions and deletions in the middle of the list.

7. **What is the `static` keyword in Java?**
   - **Answer:** The `static` keyword is used to create class-level members, which are shared among all instances of the class.
   - **Example:**
     ```java
     class MyClass {
         static int count = 0;
     }
     ```

8. **Explain the purpose of the `final` keyword in Java.**
   - **Answer:** The `final` keyword can be applied to variables, methods, and classes. It makes variables unchangeable, methods unoverridable, and classes uninheritable.
   - **Example:**
     ```java
     final int maxAttempts = 3;
     ```

9. **What is the difference between an abstract class and an interface in Java?**
   - **Answer:** An abstract class can have both abstract and concrete methods, while an interface only contains abstract methods. A class can implement multiple interfaces, but it can inherit from only one class.

10. **What is the `try-catch-finally` block used for?**
    - **Answer:** The `try-catch-finally` block is used for exception handling. Code inside the `try` block is attempted, and if an exception occurs, it is caught in the `catch` block. The `finally` block is executed regardless of whether an exception occurs or not.
    - **Example:**
      ```java
      try {
          int result = 5 / 0; // This will throw an ArithmeticException
      } catch (ArithmeticException e) {
          System.out.println("An exception occurred: " + e.getMessage());
      } finally {
          System.out.println("Finally block is executed.");
      }
      ```

11. **What is a `NullPointerException`, and how can you avoid it?**
    - **Answer:** A `NullPointerException` is thrown when you attempt to access an object's method or field that is `null`. You can avoid it by adding null checks or using the `Optional` class.
    - **Example:**
      ```java
      String text = null;
      if (text != null) {
          int length = text.length();
      }
      ```

12. **Explain the concept of method overloading in Java.**
    - **Answer:** Method overloading allows you to define multiple methods with the same name in the same class but with different parameters (number, type, or order).
    - **Example:**
      ```java
      int add(int a, int b) {
          return a + b;
      }

      double add(double a, double b) {
          return a + b;
      }
      ```

13. **What is a constructor in Java, and how is it different from a method?**
    - **Answer:** A constructor is a special method that is used to initialize objects. It has the same name as the class and is called when an object is created. Unlike methods, constructors do not have a return type.
    - **Example:**
      ```java
      class MyClass {
          public MyClass() {
              // Constructor code
          }
      }
      ```

14. **Explain the `super` keyword in Java.**
    - **Answer:** The `super` keyword is used to call a superclass's constructor, method, or member from a subclass. It is often used to access the superclass's behavior or to invoke the superclass constructor.
    - **Example:**
      ```java
      class Parent {
          void display() {
              System.out.println("Parent class method");
          }
      }

      class Child extends Parent {
          void display() {
              super.display(); // Calls the parent class method
              System.out.println("Child class method");
          }
      }
      ```

15. **What is multithreading in Java, and how is it achieved?**
    - **Answer:** Multithreading is the concurrent execution of multiple threads. In Java, it is achieved by extending the `Thread` class or implementing the `Runnable` interface.
    - **Example (using `Runnable`):**
      ```java
      class MyRunnable implements Runnable {
          public void run() {
              System.out.println("Thread is running");
          }
      }

      Thread thread = new Thread(new MyRunnable());
      thread.start();
      ```

16. **Explain the `synchronized` keyword in Java.**
    - **Answer:** The `synchronized` keyword is used to create synchronized blocks or methods, which allow only one thread to access the synchronized code block at a time, preventing concurrent data corruption.
    - **Example (synchronized method):**
      ```java
      public synchronized void synchronizedMethod() {
          // Synchronized code here
      }
      ```

17. **What is the `equals` and `hashCode` contract in Java?**
    - **Answer:** The `equals` method is used to compare the content of objects for equality, and the `hashCode` method returns an integer value that is used by data structures like HashMap. When you override `equals`, you should also override `hashCode` to maintain the contract.

18. **Explain the concept of Exception Handling in Java.**
    - **Answer:** Exception handling is a mechanism to handle runtime errors or exceptional situations. Java provides the `try-catch` block for handling exceptions.
    - **Example:**
      ```java
      try {
          // Code that may throw an exception
      } catch (ExceptionType e) {
          // Handle the exception
      }
      ```

19. **What is the purpose of the `static` block in Java?**
    - **Answer:** A `static` block is used

 to initialize static variables or perform one-time initialization tasks when a class is loaded. It runs before the class's constructor is called.
    - **Example:**
      ```java
      class MyClass {
          static {
              // Static block code
          }
      }
      ```

20. **Explain the concept of garbage collection in Java.**
    - **Answer:** Garbage collection is the automatic process of reclaiming memory occupied by objects that are no longer in use. Java has a built-in garbage collector that manages memory automatically.

Please note that these are just sample questions and answers. Depending on the position and company, the level of detail and complexity of the questions may vary. It's essential to understand the fundamentals of Java thoroughly and be prepared for a wide range of questions during an interview.