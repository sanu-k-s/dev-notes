Certainly! Here are simple notes to help you learn Object-Oriented Programming (OOP) concepts in programming with examples in C#:

1. **Object-Oriented Programming (OOP):**
   - OOP is a programming paradigm that focuses on modeling the real world using objects and classes.
   - Objects are instances of classes and encapsulate data and behavior.

2. **Class:**
   - A blueprint for creating objects.
   - Defines the structure and behavior of objects.
   
   Example in C#:
   ```csharp
   class Person
   {
       public string Name;
       public int Age;
   }
   ```

3. **Object:**
   - An instance of a class.
   - Contains data and methods defined in the class.

   Example in C#:
   ```csharp
   Person person1 = new Person();
   person1.Name = "Alice";
   person1.Age = 30;
   ```

4. **Encapsulation:**
   - The concept of bundling data and methods into a single unit (object).
   - Access to object's data is controlled by access modifiers (public, private, protected).

   Example in C#:
   ```csharp
   class BankAccount
   {
       private decimal balance;
       
       public void Deposit(decimal amount)
       {
           balance += amount;
       }
       
       public decimal GetBalance()
       {
           return balance;
       }
   }
   ```

5. **Inheritance:**
   - A mechanism that allows a class to inherit properties and behavior from another class.
   - It promotes code reuse.

   Example in C#:
   ```csharp
   class Student : Person
   {
       public int StudentID;
   }
   ```

6. **Polymorphism:**
   - The ability of objects of different classes to respond to the same method in a way that is specific to their class.
   - Achieved through method overriding and interfaces.

   Example in C# (method overriding):
   ```csharp
   class Shape
   {
       public virtual void Draw()
       {
           Console.WriteLine("Drawing a shape.");
       }
   }

   class Circle : Shape
   {
       public override void Draw()
       {
           Console.WriteLine("Drawing a circle.");
       }
   }
   ```

7. **Abstraction:**
   - The process of simplifying complex reality by modeling classes based on relevant attributes and behaviors.
   - It hides the complex implementation details.

   Example in C#:
   ```csharp
   abstract class Shape
   {
       public abstract void Draw();
   }
   ```

8. **Composition:**
   - A design principle where a class can contain objects of other classes as part of its data.

   Example in C#:
   ```csharp
   class Engine
   {
       public void Start()
       {
           Console.WriteLine("Engine started.");
       }
   }

   class Car
   {
       private Engine carEngine = new Engine();
       
       public void StartCar()
       {
           carEngine.Start();
       }
   }
   ```

These are the fundamental OOP concepts in C#. As you gain more experience, you'll explore more advanced concepts and design patterns for building complex and maintainable software.
