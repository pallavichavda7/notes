### Introduction to C#

*C#* is a modern, object-oriented programming language developed by Microsoft as part of its .NET initiative. It was designed by Anders Hejlsberg and was first released in 2000. 
* C,C++ > compiler translate code in native code.windows  native code  compiler don't run on linux, 
* to fix it simmiler like java compiler don't translate directly to machine code it translate   on byte code..  in C# compile result will IL code (intermidiate language) tarnslate into native code just in time (JIT) compilation both run on windows and linux

### C# vs .NET
* C# is a programming language
  
* .NET is a framework for building applications on windows 
* .NET * CLR - common Language Run-time 2. Class Library - 


### Architecture
Class = container some have *data & * methods

Example :  car - 
- make
- Model
- Colour
* Start()
* Move()

Namespace -  name of container 


### Basic Concepts

#### 1. *Setting Up the Environment*

- *Install Visual Studio*: Visual Studio is the most commonly used IDE for C#. Download and install it from the [official website](https://visualstudio.microsoft.com/).

#### 2. *Your First C# Program*

Let's start with a simple "Hello, World!" program.

```csharp
using System;

namespace HelloWorld
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello, World!");
        }
    }
}

```
- *using System;*: This line allows us to use classes from the System namespace.
- *namespace HelloWorld*: Namespaces are used to organize code and prevent name conflicts.
- *class Program*: A class is a blueprint for creating objects.
- *static void Main(string[] args)*: The Main method is the entry point of a C# application.
- *Console.WriteLine("Hello, World!");*: This line prints "Hello, World!" to the console.

#### 3. *Variables and Data Types*

Variables are used to store data. C# is a strongly-typed language, meaning every variable must have a type.

```csharp
int age = 25;
string name = "Alice";
bool isStudent = true;
double height = 5.8;
```

- *int*: Integer type.
- *string*: String type.
- *bool*: Boolean type.
- *double*: Double-precision floating-point type.

#### 4. *Basic Input and Output*

You can use Console.ReadLine() to read input from the user.

```csharp
Console.Write("Enter your name: ");
string name = Console.ReadLine();
Console.WriteLine("Hello, " + name);
```

### Intermediate Concepts

#### 1. *Control Structures*

- *Conditional Statements*: if, else if, else

```csharp
int number = 10;

if (number > 0)
{
    Console.WriteLine("Positive number");
}
else if (number < 0)
{
    Console.WriteLine("Negative number");
}
else
{
    Console.WriteLine("Zero");
}

```
- *Loops*: for, while, do-while

```csharp
// for loop
for (int i = 0; i < 5; i++)
{
    Console.WriteLine(i);
}

// while loop
int j = 0;
while (j < 5)
{
    Console.WriteLine(j);
    j++;
}

// do-while loop
int k = 0;
do
{
    Console.WriteLine(k);
    k++;
} while (k < 5);
```

### 2. *Methods*

Methods are used to perform a particular task. They help in code reusability.

```csharp
class Program
{
    static void Main(string[] args)
    {
        int result = Add(5, 10);
        Console.WriteLine("Sum: " + result);
    }

    static int Add(int a, int b)
    {
        return a + b;
    }
}
```

#### 3. *Arrays*

Arrays store multiple values of the same type.

```csharp
int[] numbers = { 1, 2, 3, 4, 5 };
Console.WriteLine(numbers[0]); // Output: 1
```

### Advanced Concepts

#### 1. *Object-Oriented Programming (OOP)*

- *Classes and Objects*

```csharp
class Person
{
    public string Name { get; set; }
    public int Age { get; set; }

    public void Greet()
    {
        Console.WriteLine("Hello, my name is " + Name);
    }
}
```
```csharp 
class Program
{
    static void Main(string[] args)
    {
        Person person = new Person();
        person.Name = "Alice";
        person.Age = 25;
        person.Greet(); // Output: Hello, my name is Alice
    }
}
```

- *Inheritance*

```csharp
class Animal
{
    public void Eat()
    {
        Console.WriteLine("Eating...");
    }
}

class Dog : Animal
{
    public void Bark()
    {
        Console.WriteLine("Barking...");
    }
}

class Program
{
    static void Main(string[] args)
    {
        Dog dog = new Dog();
        dog.Eat(); // Output: Eating...
        dog.Bark(); // Output: Barking...
    }
}
```

- *Polymorphism*

```csharp
class Animal
{
    public virtual void MakeSound()
    {
        Console.WriteLine("Some sound...");
    }
}

class Dog : Animal
{
    public override void MakeSound()
    {
        Console.WriteLine("Bark...");
    }
}

class Cat : Animal
{
    public override void MakeSound()
    {
        Console.WriteLine("Meow...");
    }
}

class Program
{
    static void Main(string[] args)
    {
        Animal myDog = new Dog();
        Animal myCat = new Cat();

        myDog.MakeSound(); // Output: Bark...
        myCat.MakeSound(); // Output: Meow...
    }
}
```

#### 2. *Exception Handling*

Handling runtime errors using try, catch, and finally blocks.

```csharp
try
{
    int[] numbers = { 1, 2, 3 };
    Console.WriteLine(numbers[10]);
}
catch (IndexOutOfRangeException ex)
{
    Console.WriteLine("Error: " + ex.Message);
}
finally
{
    Console.WriteLine("This block always executes.");
}
```

#### 3. *LINQ (Language Integrated Query)*

LINQ is used to query collections in a concise and readable way.

```csharp
int[] numbers = { 1, 2, 3, 4, 5 };

var evenNumbers = from number in numbers
                  where number % 2 == 0
                  select number;

foreach (var num in evenNumbers)
{
    Console.WriteLine(num);
}
```

#### 4. *Asynchronous Programming*

Asynchronous methods help in performing tasks without blocking the main thread.

```csharp
using System.Threading.Tasks;

class Program
{
    static async Task Main(string[] args)
    {
        await PrintNumbersAsync();
    }

    static async Task PrintNumbersAsync()
    {
        for (int i = 1; i <= 5; i++)
        {
            await Task.Delay(1000); // Simulate a delay
            Console.WriteLine(i);
        }
    }
}
```

### Resources for Learning C#

1. *Books*
   - C# 8.0 in a Nutshell by Joseph Albahari and Ben Albahari
   - Pro C# 8 with .NET Core by Andrew Troelsen and Philip Japikse

2. *Online Courses*
   - [Microsoft's C# Fundamentals for Absolute Beginners](https://channel9.msdn.com/Series/C-Fundamentals-for-Absolute-Beginners)
   - [Pluralsight C# Path](https://www.pluralsight.com/paths/csharp)

3. *Documentation*
   - [Microsoft C# Documentation](https://docs.microsoft.com/en-us/dotnet/csharp/)
