Certainly! C# is a statically-typed language, which means that data types must be declared before using variables. Here are some commonly used data types in C# with detailed notes and examples:

1. `int`:
   - The `int` data type represents 32-bit signed integers.
   - Example:
     ```csharp
     int age = 30;
     ```

2. `double`:
   - The `double` data type represents double-precision floating-point numbers.
   - Example:
     ```csharp
     double pi = 3.14159265359;
     ```

3. `float`:
   - The `float` data type represents single-precision floating-point numbers.
   - Example:
     ```csharp
     float temperature = 98.6f;
     ```

4. `decimal`:
   - The `decimal` data type represents high-precision decimal numbers.
   - Example:
     ```csharp
     decimal price = 19.99M;
     ```

5. `bool`:
   - The `bool` data type represents a Boolean value (true or false).
   - Example:
     ```csharp
     bool isSunny = true;
     ```

6. `char`:
   - The `char` data type represents a single Unicode character.
   - Example:
     ```csharp
     char grade = 'A';
     ```

7. `string`:
   - The `string` data type represents a sequence of characters (strings).
   - Example:
     ```csharp
     string name = "John";
     ```

8. `byte`:
   - The `byte` data type represents 8-bit unsigned integers.
   - Example:
     ```csharp
     byte data = 255;
     ```

9. `short`:
   - The `short` data type represents 16-bit signed integers.
   - Example:
     ```csharp
     short temperature = -10;
     ```

10. `long`:
    - The `long` data type represents 64-bit signed integers.
    - Example:
      ```csharp
      long population = 7_800_000_000;
      ```

11. `sbyte`:
    - The `sbyte` data type represents 8-bit signed integers.
    - Example:
      ```csharp
      sbyte temperature = -5;
      ```

12. `ushort`:
    - The `ushort` data type represents 16-bit unsigned integers.
    - Example:
      ```csharp
      ushort count = 1000;
      ```

13. `ulong`:
    - The `ulong` data type represents 64-bit unsigned integers.
    - Example:
      ```csharp
      ulong distance = 1_000_000_000;
      ```

14. `object`:
    - The `object` data type represents a reference to an object of any type.
    - Example:
      ```csharp
      object myObject = "Hello, World!";
      ```

15. `dynamic`:
    - The `dynamic` data type is a type that is resolved at runtime and can change its type.
    - Example:
      ```csharp
      dynamic value = 42;
      value = "Hello, World!";
      ```

16. `var`:
    - The `var` keyword allows the C# compiler to infer the data type of a variable at compile time.
    - Example:
      ```csharp
      var name = "Alice";
      ```

17. Custom Data Types (Classes and Structs):
    - You can create your own custom data types by defining classes and structs. These allow you to define complex data structures.
    - Example (class):
      ```csharp
      public class Person {
          public string Name { get; set; }
          public int Age { get; set; }
      }
      ```

18. `Nullable Types` (e.g., `int?`):
    - Nullable types allow value types (like int, double, etc.) to have a value of null in addition to their normal range of values.
    - Example:
      ```csharp
      int? nullableInt = null;
      ```

19. `enum`:
    - Enumerations are user-defined data types with a fixed set of named values.
    - Example:
      ```csharp
      public enum Days { Sunday, Monday, Tuesday, Wednesday, Thursday, Friday, Saturday }
      ```

20. `DateTime`:
    - The `DateTime` struct represents date and time values.
    - Example:
      ```csharp
      DateTime now = DateTime.Now;
      ```

Data types are fundamental to programming in C#. Understanding and using them correctly is essential for working with different types of data in your applications.