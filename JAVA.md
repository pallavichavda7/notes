### SHORTCUTS
* Better view  * ctrl+ k then v,
* WORD WRAP ALT+ Z
* Ctrl +K = clear console
* Cmd + k = clear console in mac
* Ctrl +R = refresh crome or console
* Ctrl +/= comment out
* /n next line print
* /p space tab print
* Ctrl + x = for the cuting the line
* 
* 

**intellij shortcuts**  
* shift + f10 = run code
* shift + f9  = debug code
* alt+ enter = fix code
* ctrl + f8 = break point set


**Java Programming: Beginner to Advanced**

---

### **1. Introduction**
- Overview of Java and its applications.
- History and significance of Java in software development.
- Explanation of how Java differs from other programming languages.

- **1:00 - Installing Java:** Guidance on setting up the Java Development Kit (JDK) and configuring the development environment.
---

### **2. Setting Up Java**
- Installing the Java Development Kit (JDK).
- Configuring environment variables.
- Setting up an Integrated Development Environment (IDE) such as IntelliJ IDEA, Eclipse, or VS Code.

**Example:**
```java
// Checking Java installation
public class Main {
    public static void main(String[] args) {
        System.out.println("Java is installed correctly!");
    }
}
```

---

### **3. Writing Your First Java Program**
- Introduction to Java syntax.
- Writing a basic 'Hello World' program.
- Explanation of main method and System.out.println().
- Running and compiling a Java program.
- **6:05 - Sample Code:** Demonstration of a simple Java program to illustrate basic syntax and structure.
- **8:37 - Writing Your First Program:** Step-by-step creation of a basic Java application, including the 'Hello World' example.


**Example:**
```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```

---

### **4. Comments in Java**
- Single-line comments (`//`).
- Multi-line comments (`/* */`).
- Documentation comments (`/** */`).
- **7:34 - Comments:** Explanation of single-line and multi-line comments in Java and their importance in code documentation.

**Example:**
```java
// This is a single-line comment
/* This is a 
   multi-line comment */
/**
 * This is a documentation comment
 */
```

---

### **5. Variables and Data Types**
- Declaring and initializing variables.
- Primitive data types (int, float, char, boolean, etc.).
- Reference data types.
- Type inference with `var`.
- **11:23 - Variables:** Introduction to variables, their declaration, initialization, and usage in Java.
- **14:00 - Data Types:** Discussion on primitive data types (byte,short,long,int, float,double, char,boolean)
non primitive data type (string)
 and their significance.


**Example:**
```java
byte number = 30;
int age = 25;
long phone = 12345678900L;
float price = 12.99f;
char grade = 'A';
boolean isJavaFun = true;
```

---

### **6. Strings in Java**
- Creating and manipulating strings.
- String methods (length, substring, replace, etc.).
- String immutability and performance considerations.
- **23:13 - Strings:** Detailed look at the String class, string manipulation methods, and common operations.

**Example:**
```java
String name = "Java Programming";
System.out.println(name.length()); // 16
System.out.println(name.toUpperCase()); //JAVA PROGRAMMING
System.out.println(name.toLowercase());//java programming

```

- new key word use for create new string
```java
String name = "Bombay";
// classes k object new keyword
String city = new String( "Mumbai");
System.out.println(name);//Bombay
System.out.println(city);//Mumbai

```
- concanating 
```java
String name1 = "Pallavi";
String name2 = "Chavda";
String fullname = name1 + " " + name2;
System.out.println(fullname);//Pallavi Chavda
```
---
- printing one character 
```java
String name = "Pallavi";
System.out.println(name.charAt(1));//a
```
- replacing 
```java
String name = "Pallavi";
String name2 = name.replace('P', 'S');
System.out.println(name2);//Sallavi
```
**java strings are immutable - no change in orignal string if change is needed create new string**
- sub string index printing 
* 17 will not include thats why 18 taken as index 
```java
String name = "Pallavi and Bombay";
System.out.println(name.substring(0,18));
``` 
### **7. Arrays in Java**
- Declaring and initializing arrays.
- Accessing array elements.
- Multi-dimensional arrays.
- Array methods and operations.
** if we try to print array it will create gargen code insted of elements printing
```java
// type [] name = new data type[ no];
int[] marks = new int[3];
marks[0] = 97;
marks[1] = 85;
marks[2] = 88;

System.out.println(marks[0]);
```
** if we don't declare the array by defalut it will have null values
- **29:33 - Arrays:** Explanation of arrays, their declaration, initialization, and traversal techniques.

**Example:**
```java
int[] numbers = {1, 2, 3, 4, 5};
System.out.println(numbers[2]); // Output: 3
```
- array length
```java
int[] marks = new int[3];
marks[0] = 97;
marks[1] = 85;
marks[2] = 88;

System.out.println(marks.length);//3
```
- array sort
```java
// import java.util.Arrays;
// in first line
int[] marks = new int[3];
    marks[0] = 97;
    marks[1] = 85;
    marks[2] = 88;

    System.out.println(marks[0]);
    Arrays.sort(marks);
    System.out.println(marks[0]);
```
- array
```java
// if you know how many value you have to store in it you can also write the code to create array
int[] marks = {97,98,95};
```
- 2d array
```java
     int [] marks = {97,98,95};

     int [][] finalMarks = {{97,98,95},{95,95,98}};
        System.out.println(finalMarks[1][1]); // 95
```
---

### **8. Type Casting in Java**
- shifting data from small container to big container over flow when big data type will stored in to small data type
- Implicit (widening) and explicit (narrowing) casting.
- Converting between different data types.

- **42:32 - Casting:** Understanding type casting, both implicit and explicit, and its applications.

**Example:**
```java
int num = 10;
double newNum = num; // Implicit casting

double val = 9.78;
int intVal = (int) val; // Explicit casting
```
```java
    double price = 100.00;//8 byte
    double finalPrice = price + 18;
    System.out.println(finalPrice);//118.0
        // implicit casting
        
    int p = 100; // loose data is okay
    int fp = p + (int)18.18;// data trunked - removed
    System.out.println(fp);//118 
```

---

### **9. Constants in Java**
- Declaring constants using `final` keyword.
- Importance of constants in preventing data modification.
- **48:05 - Constants:** Use of the 'final' keyword to define constants and their role in maintaining immutable values.
**Example:**
```java
final double PI = 3.14159;
System.out.println(PI);
```

---

### **10. Operators in Java**
- Arithmetic, assignment, and comparison operators.
- Logical operators (`&&`, `||`, `!`).
- **49:52 - Operators (Arithmetic & Assignment):** Overview of various operators in Java, including arithmetic, assignment, and their usage.

**Example:** arithmetic
```java
double a = 10, b = 5;
    System.out.println(a + b);// 15
    System.out.println(a - b);//5
    System.out.println(a * b);//50
    System.out.println(a / b);//2
    System.out.println(a % b);//0
    System.out.println(a > b);//true
```
- unary operators -1 = -- ,+1 = ++,
```java
int numb = 5;
++numb;// before change
//numb++; after change
System.out.println(numb);//6

```
---

### **11. Math Class in Java**
- Using built-in mathematical functions.
- Common methods (abs, sqrt, pow, etc.).
- **57:59 - Math Class:** Introduction to the Math class and its methods for performing mathematical operations.

**Example:**
```java
System.out.println(Math.sqrt(25)); // 5.0
System.out.println(Math.pow(2, 3)); // 8.0
System.out.println(Math.floor(485.99));//485.0
System.out.println((double) Math.random());//0.67725526323891
System.out.println( Math.abs(18.9));//18.9
```
- min max functions
```java
System.out.println(Math.max(5,6));//6
System.out.println(Math.min(8,9));//8
```
---

### **12. Taking User Input**
- Using the `Scanner` class.
- Reading different data types from user input.
- **1:00:45 - Taking Input:** Methods to capture user input using the Scanner class.

**Example:**
```java
import java.util.Scanner;
Scanner scanner = new Scanner(System.in);
System.out.print("Enter your name: ");
String name = scanner.nextLine();//line will input full line
System.out.println("Hello, " + name);

Scanner sc = new Scanner(System.in);//object
        System.out.println("enter your age: ");
        int age = sc.nextInt();//function
        System.out.println(age);
```

---

### **13. Conditional Statements**
- `if`, `else if`, `else` statements.
- Using `switch-case` for multiple conditions.
- **1:04:48 - Comparison Operators:** Explanation of comparison operators and their role in decision-making processes.
```java
// a == b
//a != b
// a < b
// a < b
// a <= b
// a >= b
```
- **1:07:10 - Conditional Statements (if-else):** Detailed look at if-else statements and their syntax for branching logic.
```java
    boolean isSunUp = false;
    if(isSunUp == true)
        System.out.println("day");
        else
        System.out.println("night");
```
```java
int age = 30;
     if(age > 18)
        System.out.println("can vote");
    else
        System.out.println("can not vote");
```


- **1:09:00 - Logical Operators:** Discussion on logical operators (AND, OR, NOT) and their usage in combining conditions.
```java
// && t + t = t
    int a = 30;
    int b = 40;

    if(a < 50 && b < 50)
    System.out.println("both less than 50");
// || t + f = t
    int a = 30;
    int b = 40;
if(a < 50 || b <50)
System.out.println("both less than 50");
// ! 
boolean isAdult = false;
if (!isAdult)
System.out.println("is adult");
else
System.out.println("not adult");
```


- **1:17:55 - Conditional Statements (switch):** Introduction to the switch statement as an alternative to multiple if-else conditions.
**Example:**
```java
int age = 18;
if (age >= 18) {
    System.out.println("Adult");
} else {
    System.out.println("Minor");
}
```
```java
import java.util.Scanner;

Scanner sc = new Scanner(System.in);

        int cash = sc.nextInt();
        if (cash<10){
            System.out.println("can't buy anything");
            System.out.println("get more cash");
        } else if (cash> 10 && cash < 50) {
            System.out.println("can get 1 thing");
        }
        else {
            System.out.println("can get both");
        }
```
#### switch case
```java
int day = 3;
    switch (day){
        case 1 :
            System.out.println("monday");
            break;
        case 2 :
            System.out.println("tuesday");
            break;
        case 3 :
            System.out.println("wednesday");
            break;
        case 4 :
            System.out.println("thursday");
            break;
        case 5 :
            System.out.println("friday");
            break;
        case 6 :
            System.out.println("saturday");
            break;
        default:
            System.out.println("sunday");
    }
```
---

### **14. Loops in Java**
- `for`, `while`, and `do-while` loops.
- Loop control statements (`break`, `continue`).
- **1:21:29 - Loops:** Comprehensive coverage of looping constructs like for, while, and do-while loops.


**Example:**
```java
for (int i = 0; i < 5; i++) {
    System.out.println("Iteration " + i);
}
```
```java
int j = 10;
    while(j >= 1){
    System.out.println(j);
    j--;
    }

```
```java
int k = 10;
do{
    System.out.println(k);
    k--;
}
while(k >= 1);
```
```java
import java.util.Scanner;
Scanner sc = new Scanner(System.in);
    int number = 0;

    do {
        System.out.println("input a number");
        number = sc.nextInt();
        System.out.println(number);
    }while ( number >= 0);
        System.out.println("the end");

```
---

- **1:34:13 - Break & Continue:** Explanation of break and continue statements to control loop execution flow.
```java
int i = 0;
    while(true){
        System.out.println(i);
        i++;
        if(i>5){
            break;
        }
    }
```
```java
int i = 0;
        while(true){
            if (i == 3){
                i ++;
                continue;
            }
            System.out.println(i);
            i++;
            if(i > 5){
                break;
            }
        }
```        


### **15. Exception Handling**
- Using `try`, `catch`, and `finally` blocks.
- **1:40:29 - Exception Handling (try-catch):** Basics of exception handling using try-catch blocks to manage runtime errors.

**Example:**
```java
try {
    int result = 10 / 0;
} catch (ArithmeticException e) {
    System.out.println("Error: Division by zero");
}
```
```java
int [] marks = { 97,98,95};
        try{
            System.out.println(marks[5]);
        } catch (Exception exception) {
            // do something  after catching it
        }
        System.out.println("the system is working on it");
```
---

### **16. Functions/Methods in Java**
- Defining and calling methods.
- Method parameters and return types.
- example = button of remote method ,remote is function, remote is class
- **1:46:46 - Functions/Methods:** Creation and invocation of methods, including parameter passing and return types.

**Example:**
```java
public static int add(int a, int b) {
    return a + b;
}
System.out.println(add(5, 10)); // 15
```

---

### **17. Mini-Project**
- Applying all learned concepts in a real-world Java project.
- **1:56:18 - Mini-Project:** A practical project to apply the concepts learned throughout the tutorial.


**Example Project: Simple Calculator**
```java
import java.util.Scanner;
public class Calculator {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter first number: ");
        double num1 = scanner.nextDouble();
        System.out.print("Enter second number: ");
        double num2 = scanner.nextDouble();
        System.out.println("Sum: " + (num1 + num2));
    }
}
```

---
# ANDROID STUDIO

- 2008 Introduction popular oprating system
- 2.5 Bilion ANDROID
- 1. install android STUDIO
- 2. basic of android STUDIO
- 3. 


- new project open with activity settings 
- bottoms activity navigations example instagram
- view model recycler view
- full screen activity gaming 
- master details flow song and 
- navigations  drawer
- gogle maps activity - uber ,ola
- log in activity
- scroling - bloger app , news app 
- taged activity , 
- c++ activity
- smart watch activity
- tv live streaming activity
- messages services send messages
- empty activity
 
