# Java Programming :

Java is a versatile, object-oriented programming language designed for cross-platform compatibility. It allows developers to write code once and run it anywhere (WORA), making it platform-independent. Here are some key points about Java:

- Origin and Release:

  - Developed by James Gosling at Sun Microsystems, released in 1995.
  - Acquired by Oracle Corporation.

- Key Features:

  - Class-based and object-oriented.
  - Syntax similar to C and C++ but with fewer low-level facilities.

- Popularity:

  - As of 2019, one of the most popular languages on GitHub with 9 million developers.

- Compilation and Execution:

  - Applications compiled to bytecode for Java Virtual Machine (JVM) execution.

- Release Cycle:

  - Major release every six months, Long-Term Support (LTS) release every three years.

- Security Concerns:

  - Uninstalling older versions recommended due to unresolved security issues.

- Latest Version:

  - Java 16, released in March 2021, with Java 17 scheduled for September 2021.

- Licensing:

  - Java technologies mostly released under the GNU General Public License.

- Alternative Implementations:
  - Various alternatives like GNU Compiler for Java, GNU Classpath, and IcedTea-Web.

---

## table of contents :

Certainly! I have removed the duplicate entries in the table of contents. Here's the revised version:

## Table of Contents:

### 1. Core Java Concepts:

- Variables and Data Types:

  - Primitive Data Types
  - Wrapper Classes
  - Reference Data Types

- Operators:
- Control Flow Statements:
- Arrays:
- Methods:

### 2. Object-Oriented Programming (OOP):

- Classes and Objects:
- Encapsulation:
- Polymorphism:
  - Overloading
  - Overriding
- Constructors:
- Inheritance:
- Abstract Classes:
- Interfaces:
- Abstraction and Interfaces:
- Packages:
- Access Modifiers:
- Static Keyword:
- Final Keyword:
- Object Class:
- String Class:
- Wrapper Classes:
- Autoboxing and Unboxing:
- Enum Types:
- Annotations:
- Lambda Expressions:
- Functional Interfaces:
- Method References:
- Default Methods:
- Optional Class:
- New Date/Time API:
- Streams:
- Collections:
- Multithreading:
- Synchronization:
- Serialization:
- Networking:
- JDBC:
- Java Beans:
- Reflection API:
- Generics:
- Annotations:
- Internationalization:
- Java 8 Features:
- Java 9 Features:
- Java 10 Features:
- Java 11 Features:
- Java 12 Features:
- Java 13 Features:
- Java 14 Features:
- Java 15 Features:
- Java 16 Features:
- Java 17 Features:

### 3. Collections and Generics:

- Collections Framework:
- Generics:

### 4. Exception Handling:

- Errors and Exceptions:

### 5. Input/Output (I/O):

- File I/O:
- Console I/O:

### 6. Threads and Concurrency:

- Multithreading:

### 7. Networking:

- Sockets:
- URLs and URIs:

### 8. Database Programming (Optional):

- JDBC:

### 9. Java 8 Features:

- Lambda Expressions:
- Streams:
- Functional Interfaces:
- Method References:
- Default Methods:
- Optional Class:
- New Date/Time API:

### 10. Java 9 Features:

- JShell:
- Private Methods in Interfaces:
- Collection Factory Methods:

### 11. Java 10 Features:

- Local Variable Type Inference:

### 12. Java 11 Features:

- String Methods:
- Files Methods:
- Predicate Methods:
- Optional Methods:
- Stream Methods:
- Collectors Methods:

### 13. Java 12 Features:

- Switch Expressions:

### 14. Java 13 Features:

- Text Blocks:

### 15. Java 14 Features:

- Records:

### 16. Java 15 Features:

- Sealed Classes:

### 17. Java 16 Features:

- Pattern Matching for instanceof:
- Records:
- Local Variable Type Inference:
- Garbage Collection:

This version should be free of duplicate entries.

## 1. Core Java Concepts:

### Variables and Data Types:

#### Primitive Data Types:

| Data Type | Size (in bits) | Default Value | Default Value (for fields) |
| --------- | -------------- | ------------- | -------------------------- |
| byte      | 8              | 0             | 0                          |
| short     | 16             | 0             | 0                          |
| int       | 32             | 0             | 0                          |
| long      | 64             | 0L            | 0L                         |
| float     | 32             | 0.0f          | 0.0f                       |
| double    | 64             | 0.0d          | 0.0d                       |
| char      | 16             | '\u0000'      | '\u0000'                   |

Example:

```java
public class Main {
    public static void main(String[] args) {
        byte b = 5;
        short s = 10;
        int i = 20;
        long l = 50L;
        float f = 0.5f;
        double d = 0.5d;
        char c = 'A';
        boolean bool = true;

        System.out.println("byte: " + b);
        System.out.println("short: " + s);
        System.out.println("int: " + i);
        System.out.println("long: " + l);
        System.out.println("float: " + f);
        System.out.println("double: " + d);
        System.out.println("char: " + c);
        System.out.println("boolean: " + bool);
    }
}

```

Output:

```java
byte: 5
short: 10
int: 20
long: 50
float: 0.5
double: 0.5
char: A
boolean: true
```

#### Wrapper Classes:

| Primitive Data Type | Wrapper Class |
| ------------------- | ------------- |
| byte                | Byte          |
| short               | Short         |
| int                 | Integer       |
| long                | Long          |
| float               | Float         |
| double              | Double        |
| char                | Character     |
| boolean             | Boolean       |

Example:

```java
public class Main {
    public static void main(String[] args) {
        Byte b = 5;
        Short s = 10;
        Integer i = 20;
        Long l = 50L;
        Float f = 0.5f;
        Double d = 0.5d;
        Character c = 'A';
        Boolean bool = true;

        System.out.println("Byte: " + b);
        System.out.println("Short: " + s);
        System.out.println("Integer: " + i);
        System.out.println("Long: " + l);
        System.out.println("Float: " + f);
        System.out.println("Double: " + d);
        System.out.println("Character: " + c);
        System.out.println("Boolean: " + bool);
    }
}
```

Output:

```java
Byte: 5
Short: 10
Integer: 20
Long: 50
Float: 0.5
Double: 0.5
Character: A
Boolean: true
```

#### Reference Data Types:

| Reference Data Type | Size (in bits) | Default Value | Default Value (for fields) |
| ------------------- | -------------- | ------------- | -------------------------- |
| String              | 64             | null          | null                       |

Example:

```java
public class Main {
    public static void main(String[] args) {
        String str = "Hello World!";
        System.out.println(str);
    }
}
```

Output:

```java
Hello World!
```

### Operators:

| Operator Type    | Operators                                           |
| ---------------- | --------------------------------------------------- |
| Arithmetic       | +, -, \*, /, %, ++, --                              |
| Bitwise          | &, \|, ^, ~, <<, >>, >>>                            |
| Relational       | ==, !=, >, <, >=, <=                                |
| Logical          | &&, \|\|, !                                         |
| Assignment       | =, +=, -=, \*=, /=, %=, &=, \|=, ^=, <<=, >>=, >>>= |
| Ternary          | ?:                                                  |
| Null             | ??                                                  |
| instanceof       | instanceof                                          |
| Method Reference | ::                                                  |

Example:
Arithmetic

```java
public class Main {
    public static void main(String[] args) {
        int a = 5;
        int b = 2;

        System.out.println("a + b = " + (a + b));
        System.out.println("a - b = " + (a - b));
        System.out.println("a * b = " + (a * b));
        System.out.println("a / b = " + (a / b));
        System.out.println("a % b = " + (a % b));
        System.out.println("a++ = " + (a++));
        System.out.println("++a = " + (++a));
        System.out.println("b-- = " + (b--));
        System.out.println("--b = " + (--b));
    }
}
```

Output:

```java
a + b = 7
a - b = 3
a * b = 10
a / b = 2
a % b = 1
a++ = 5
++a = 7
b-- = 2
--b = 0
```

Example:
Bitwise

```java
public class Main {
    public static void main(String[] args) {
        int a = 5;
        int b = 2;

        System.out.println("a & b = " + (a & b));
        System.out.println("a | b = " + (a | b));
        System.out.println("a ^ b = " + (a ^ b));
        System.out.println("~a = " + (~a));
        System.out.println("a << b = " + (a << b));
        System.out.println("a >> b = " + (a >> b));
        System.out.println("a >>> b = " + (a >>> b));
    }
}
```

Output:

```java
a & b = 0
a | b = 7
a ^ b = 7
~a = -6
a << b = 20
a >> b = 1
a >>> b = 1
```

Example:
Relational

```java
public class Main {
    public static void main(String[] args) {
        int a = 5;
        int b = 2;

        System.out.println("a == b: " + (a == b));
        System.out.println("a != b: " + (a != b));
        System.out.println("a > b: " + (a > b));
        System.out.println("a < b: " + (a < b));
        System.out.println("a >= b: " + (a >= b));
        System.out.println("a <= b: " + (a <= b));
    }
}
```

Output:

```java
a == b: false
a != b: true
a > b: true
a < b: false
a >= b: true
a <= b: false
```

Example:
Logical

```java
public class Main {
    public static void main(String[] args) {
        boolean a = true;
        boolean b = false;

        System.out.println("a && b: " + (a && b));
        System.out.println("a || b: " + (a || b));
        System.out.println("!a: " + (!a));
    }
}
```

Output:

```java
a && b: false
a || b: true
!a: false
```

Example:
Assignment

```java
public class Main {
    public static void main(String[] args) {
        int a = 5;
        int b = 2;

        System.out.println("a = " + (a));
        System.out.println("a += b: " + (a += b));
        System.out.println("a -= b: " + (a -= b));
        System.out.println("a *= b: " + (a *= b));
        System.out.println("a /= b: " + (a /= b));
        System.out.println("a %= b: " + (a %= b));
        System.out.println("a &= b: " + (a &= b));
        System.out.println("a |= b: " + (a |= b));
        System.out.println("a ^= b: " + (a ^= b));
        System.out.println("a <<= b: " + (a <<= b));
        System.out.println("a >>= b: " + (a >>= b));
        System.out.println("a >>>= b: " + (a >>>= b));
    }
}
```

Output:

```java
a = 5
a += b: 7
a -= b: 5
a *= b: 10
a /= b: 5
a %= b: 1
a &= b: 0
a |= b: 2
a ^= b: 0
a <<= b: 0
a >>= b: 0
a >>>= b: 0
```

Example:
Ternary

```java
public class Main {
    public static void main(String[] args) {
        int a = 5;
        int b = 2;

        System.out.println("a > b ? a : b: " + (a > b ? a : b));
    }
}
```

Output:

```java
a > b ? a : b: 5
```

Example:
Null

```java
public class Main {
    public static void main(String[] args) {
        Integer a = null;
        Integer b = 2;

        System.out.println("a ?? b: " + (a ?? b));
    }
}
```

Output:

```java
a ?? b: 2
```

Example:
instanceof

```java
public class Main {
    public static void main(String[] args) {
        Integer a = 5;

        System.out.println("a instanceof Integer: " + (a instanceof Integer));
    }
}
```

Output:

```java
a instanceof Integer: true
```

Example:
Method Reference

```java
import java.util.Arrays;

public class Main {
    public static void main(String[] args) {
        String[] arr = {"Hello", "World"};

        Arrays.stream(arr).forEach(System.out::println);
    }
}
```

Output:

```java
Hello
World
```

### Control Flow Statements:

| Statement Type | Statements                                       |
| -------------- | ------------------------------------------------ |
| Conditional    | if, if-else, if-else-if, switch                  |
| Loop           | for, while, do-while                             |
| Jump           | break, continue, return                          |
| Exception      | try-catch, try-catch-finally, try-with-resources |

Example:
if-else-if

```java
public class Main {
    public static void main(String[] args) {
        int n = 5;

        if (n > 0) {
            System.out.println("n is positive");
        } else if (n < 0) {
            System.out.println("n is negative");
        } else {
            System.out.println("n is zero");
        }
    }
}
```

Output:

```java
n is positive
```

Example:
switch

```java
public class Main {
    public static void main(String[] args) {
        int n = 5;

        switch (n) {
            case 1:
                System.out.println("n is 1");
                break;
            case 2:
                System.out.println("n is 2");
                break;
            case 3:
                System.out.println("n is 3");
                break;
            default:
                System.out.println("n is not 1, 2, or 3");
        }
    }
}
```

Output:

```java
n is not 1, 2, or 3
```

Example:
for

```java
public class Main {
    public static void main(String[] args) {
        for (int i = 0; i < 5; i++) {
            System.out.println(i);
        }
    }
}
```

Output:

```java
0
1
2
3
4
```

Example:
while

```java
public class Main {
    public static void main(String[] args) {
        int i = 0;

        while (i < 5) {
            System.out.println(i);
            i++;
        }
    }
}
```

Output:

```java
0
1
2
3
4
```

Example:
do-while

```java
public class Main {
    public static void main(String[] args) {
        int i = 0;

        do {
            System.out.println(i);
            i++;
        } while (i < 5);
    }
}
```

Output:

```java
0
1
2
3
4
```

Example:
break

```java
public class Main {
    public static void main(String[] args) {
        for (int i = 0; i < 5; i++) {
            if (i == 3) {
                break;
            }
            System.out.println(i);
        }
    }
}
```

Output:

```java
0
1
2
```

Example:
continue

```java
public class Main {
    public static void main(String[] args) {
        for (int i = 0; i < 5; i++) {
            if (i == 3) {
                continue;
            }
            System.out.println(i);
        }
    }
}
```

Output:

```java
0
1
2
4
```

Example:
return

```java
public class Main {
    public static void main(String[] args) {
        System.out.println("Before return statement");

        return;

        // Unreachable statement
        // System.out.println("After return statement");
    }
}
```

Output:

```java
Before return statement
```

Example:
try-catch

```java
public class Main {
    public static void main(String[] args) {
        try {
            int[] arr = new int[5];
            System.out.println(arr[5]);
        } catch (Exception e) {
            System.out.println("Exception caught!");
        }
    }
}
```

Output:

```java
Exception caught!
```

Example:
try-catch-finally

```java
public class Main {
    public static void main(String[] args) {
        try {
            int[] arr = new int[5];
            System.out.println(arr[5]);
        } catch (Exception e) {
            System.out.println("Exception caught!");
        } finally {
            System.out.println("Finally block executed!");
        }
    }
}
```

Output:

```java
Exception caught!
Finally block executed!
```

Example:
try-with-resources

```java
import java.io.*;

public class Main {
    public static void main(String[] args) {
        try (BufferedReader br = new BufferedReader(new FileReader("input.txt"))) {
            String line;
            while ((line = br.readLine()) != null) {
                System.out.println(line);
            }
        } catch (IOException e) {
            System.out.println("IOException caught!");
        }
    }
}
```

Output:

```java
Hello World!
```

### Arrays:

Arrays are used to store multiple values in a single variable. Each value in an array is called an element. Arrays can be of primitive data types or reference data types.
Types of Arrays: One-Dimensional Arrays, Two-Dimensional Arrays, Multi-Dimensional Arrays.

Example:

```java
public class Main {
    public static void main(String[] args) {
        int[] arr = new int[5];

        for (int i = 0; i < 5; i++) {
            arr[i] = i;
        }

        for (int i = 0; i < 5; i++) {
            System.out.println(arr[i]);
        }
    }
}
```

Output:

```java
0
1
2
3
4
```

### Methods:

Methods are used to perform certain actions, and they are also known as functions. Methods are used to reuse code: define the code once, and use it many times. Methods are also known as functions.

Example:

```java
public class Main {
    public static void main(String[] args) {
        System.out.println("Hello World!");
    }
}
```

Output:

```java
Hello World!
```

Certainly! Let's break down each of the four pillars of Object-Oriented Programming (OOP) into subpoints:

---

## 2. Object-Oriented Programming (OOP):

### Classes and Objects:

Classes serve as blueprints for creating objects, which are instances of classes. Classes can have fields (attributes) and methods (functions).

Types of Classes:

- Concrete Classes: Can be instantiated and may be either a subclass or superclass, but not an abstract class.

  ```java
  public class Car {
      String brand;
      int year;

      void start() {
          System.out.println("Car started!");
      }
  }
  ```

- Abstract Classes: Cannot be instantiated and can include abstract methods without a body.

  ```java
  abstract class Shape {
      abstract void draw(); // Abstract method with no implementation
  }
  ```

- Interface Types: Similar to abstract classes, but all methods are abstract and can be implemented by multiple classes.

  ```java
  interface Drawable {
      void draw();
  }
  ```

### Encapsulation:

Encapsulation involves bundling code and data into a single unit, hiding implementation details from users. It helps in maintaining the integrity of the data.

```java
public class BankAccount {
    private double balance;

    public void deposit(double amount) {
        balance += amount;
    }

    public void withdraw(double amount) {
        if (amount <= balance) {
            balance -= amount;
        } else {
            System.out.println("Insufficient funds.");
        }
    }

    public double getBalance() {
        return balance;
    }
}
```

### Polymorphism:

Polymorphism allows objects to take on multiple forms. It can be achieved through method overloading or method overriding.

Example - Method Overloading:

```java
public class Calculator {
    int add(int a, int b) {
        return a + b;
    }

    double add(double a, double b) {
        return a + b;
    }
}
```

Example - Method Overriding:

```java
class Animal {
    void sound() {
        System.out.println("Animal makes a sound");
    }
}

class Dog extends Animal {
    @Override
    void sound() {
        System.out.println("Dog barks");
    }
}
```

### Constructors:

Constructors initialize objects when they are created. They have the same name as the class and no return type.

```java
public class Person {
    String name;
    int age;

    // Constructor
    public Person(String n, int a) {
        name = n;
        age = a;
    }
}
```

### Inheritance:

Inheritance allows a new class (subclass) to inherit attributes and methods from an existing class (superclass).

```java
class Vehicle {
    void start() {
        System.out.println("Vehicle started!");
    }
}

class Car extends Vehicle {
    void accelerate() {
        System.out.println("Car accelerating!");
    }
}
```

### Abstract Classes:

Abstract classes cannot be instantiated and can have abstract (unimplemented) and concrete (implemented) methods.

```java
abstract class Shape {
    int sides;

    Shape(int s) {
        sides = s;
    }

    abstract double calculateArea();
}

class Circle extends Shape {
    double radius;

    Circle(double r) {
        super(0); // Circles have 0 sides
        radius = r;
    }

    @Override
    double calculateArea() {
        return Math.PI * radius * radius;
    }
}
```

### Types:

Types represent the nature of a variable, indicating what kind of values it can hold.

Example - Primitive Types:

```java
int number = 42;        // Integer type
double pi = 3.14;       // Floating-point type
boolean isTrue = true;   // Boolean type
char grade = 'A';        // Character type
```

Example - Reference Types:

```java
String message = "Hello";   // String type
Car myCar = new Car();       // User-defined class type
List<Integer> numbers = new ArrayList<>();  // Generic type (List of Integers)
```

### Four Pillars of OOP:

#### 1. Encapsulation:

Encapsulation is the bundling of data (attributes) and the methods (functions) that operate on the data into a single unit, often referred to as a class. This helps in hiding the internal details of how an object works and only exposing what is necessary.

- Benefits:
  - Data Protection: Prevents direct access to data, ensuring that it can only be modified through well-defined methods.
  - Code Organization: Keeps related code and data together, improving maintainability.

#### 2. Abstraction:

Abstraction is the process of simplifying complex systems by modeling classes based on the essential properties and behaviors they share. It involves defining abstract classes and methods that can be implemented by concrete classes.

- Benefits:
  - Simplification: Focuses on essential features while hiding unnecessary details.
  - Flexibility: Allows changes to the implementation without affecting the external code.

#### 3. Inheritance:

Inheritance allows a new class (subclass) to inherit attributes and methods from an existing class (superclass). It promotes code reuse and establishes a relationship between classes.

- Benefits:
  - Code Reusability: Subclasses can reuse code from their superclass, reducing redundancy.
  - Relationships: Establishes relationships between classes, creating a hierarchy.

#### 4. Polymorphism:

Polymorphism allows objects to take on multiple forms. It can be achieved through method overloading (compile-time polymorphism) and method overriding (runtime polymorphism).

- Benefits:
  - Flexibility: Enables a single interface to represent various types of objects.
  - Extensibility: Allows adding new functionality without modifying existing code.

---

## 3. Collections and Generics:

### Collections Framework:

The Collections Framework serves as a comprehensive architecture for representing and manipulating collections in Java. It comprises interfaces, implementations, and algorithms tailored for diverse collection types.

#### Interfaces:

- Collection: Represents a group of objects, known as its elements.
- List: An ordered collection allowing duplicate elements.
- Set: A collection prohibiting duplicate elements.
- Queue: Holds elements for processing.
- Deque: Holds elements with support for both First-In-First-Out (FIFO) and Last-In-First-Out (LIFO).
- Map: Maps keys to values, disallowing duplicate keys.
- SortedMap: Maintains mappings in ascending key order.
- NavigableMap: Supports efficient navigation methods.
- SortedSet: Maintains elements in ascending order.
- NavigableSet: Supports efficient navigation methods.

#### Implementations:

- ArrayList: Resizable array supporting random access.
- LinkedList: Doubly-linked list supporting sequential access.
- Vector: Resizable array supporting random access, synchronized.
- Stack: Last-In-First-Out (LIFO) stack.
- HashSet: Set using a hash table for storage.
- LinkedHashSet: Set using a hash table with predictable iteration order.
- TreeSet: Set using a tree for storage, sorted by a comparator or natural ordering.
- PriorityQueue: Queue ordering elements by natural ordering or a comparator.
- ArrayDeque: Double-ended queue supporting insertion and removal at both ends.
- HashMap: Map using a hash table for storage.
- LinkedHashMap: Map using a hash table with predictable iteration order.
- TreeMap: Map using a tree for storage, sorted by a comparator or natural ordering.
- WeakHashMap: Map using a hash table with weak keys.
- IdentityHashMap: Map using a hash table with equality based on reference equality.

#### Algorithms:

- Sorting: Sorts a list based on natural ordering or a comparator.
- Shuffling: Randomly permutes list elements.
- Searching: Searches for an element in a collection.
- Min/Max: Finds the minimum or maximum element in a collection.
- Comparison: Compares two elements for order.
- Iterator: Iterates over elements in a collection.
- ListIterator: Iterates over elements in a list.
- Enumeration: Enumerates elements in a collection.

### Generics:

Generics enable the parameterization of types when defining classes, interfaces, and methods in Java. They offer compile-time type safety and eliminate the need for casting.

Example:

```java
public class Main {
    public static void main(String[] args) {
        List<Integer> numbers = new ArrayList<>();
        numbers.add(1);
        numbers.add(2);
        numbers.add(3);

        for (int i : numbers) {
            System.out.println(i);
        }
    }
}
```

Output:

```java
1
2
3
```

## 4. Exception Handling:

### Errors and Exceptions:

Errors and exceptions are abnormal conditions that disrupt the normal flow of execution. Errors are caused by the environment in which the application is running, while exceptions are caused by the application itself.

#### Types of Errors:

- OutOfMemoryError: Thrown when the Java Virtual Machine cannot allocate an object due to running out of memory, and no more memory can be made available by the garbage collector.
- StackOverflowError: Thrown when a stack overflow occurs because an application recurses too deeply.
- NoClassDefFoundError: Thrown when the Java Virtual Machine or a ClassLoader instance tries to load in the definition of a class, but no definition for the class with the specified name could be found.

#### Types of Exceptions:

- RuntimeException: Exceptions during JVM's normal operation.
- IOException: Exceptions during input and output operations.
- ClassNotFoundException: Loading a class fails.
- InterruptedException: Thread waiting, sleeping, or occupied is interrupted.
- NoSuchMethodException: A specific method cannot be found.
- NoSuchFieldException: A specific field cannot be found.
- IllegalAccessException: Illegal access to a class, field, or method.
- InstantiationException: Cannot instantiate a class.
- ArithmeticException: Arithmetic operation exception.
- ArrayIndexOutOfBoundsException: Array access with an illegal index.
- ArrayStoreException: Storing the wrong type of object in an array.
- ClassCastException: Casting an object to an incompatible class.
- IllegalArgumentException: Illegal or inappropriate argument.
- IllegalMonitorStateException: Illegal monitor operation.
- IllegalStateException: Method invoked at an illegal time.
- IllegalThreadStateException: Thread not in an appropriate state.
- IndexOutOfBoundsException: Index out of range.
- NegativeArraySizeException: Creating an array with a negative size.
- NullPointerException: Null reference where an object is required.
- SecurityException: Security infrastructure exception.
- StringIndexOutOfBoundsException: String-related method exception.
- UnsupportedOperationException: Requested operation not supported.

#### Example:

```java
public class ExceptionHandlingExample {
    public static void main(String[] args) {
        try {
            int[] arr = new int[5];
            System.out.println(arr[5]); // ArrayIndexOutOfBoundsException

            int result = 10 / 0; // ArithmeticException

            String str = null;
            System.out.println(str.length()); // NullPointerException

            // Example of IOException (Checked Exception)
            BufferedReader reader = new BufferedReader(new FileReader("nonexistentfile.txt"));
            String line = reader.readLine(); // IOException

        } catch (ArrayIndexOutOfBoundsException e) {
            System.out.println("ArrayIndexOutOfBoundsException caught!");
        } catch (ArithmeticException e) {
            System.out.println("ArithmeticException caught!");
        } catch (NullPointerException e) {
            System.out.println("NullPointerException caught!");
        } catch (IOException e) {
            System.out.println("IOException caught!");
        } catch (Exception e) {
            System.out.println("Generic Exception caught!");
        } finally {
            System.out.println("Finally block always executes.");
        }
    }
}
```

Output:

```java
ArrayIndexOutOfBoundsException caught!
ArithmeticException caught!
NullPointerException caught!
IOException caught!
Finally block always executes.
```

This example demonstrates the handling of specific exceptions such as `ArrayIndexOutOfBoundsException`, `ArithmeticException`, `NullPointerException`, and a generic `IOException`. The `finally` block is included to emphasize its execution regardless of the exception type.

## 5. Input/Output (I/O):

### File I/O:

File I/O (Input/Output) is the process of reading from and writing to files. It is used to store data persistently.

#### Types of Streams:

- Byte Streams: Used to perform input and output of 8-bit bytes.
- Character Streams: Used to perform input and output for 16-bit unicode.
- Buffered Streams: Used to improve the performance of input and output.
- Scanning and Formatting: Used to parse and generate formatted output.
- Data Streams: Used to perform input and output of primitive data types.
- Object Streams: Used to perform input and output of objects.
- Sequence Streams: Used to write data sequentially.
- Pipe Streams: Used to transfer data between threads.

#### Types of Channels:

- File Channels: Used to read data from and write data to files.
- Datagram Channels: Used to read and write datagrams.
- Socket Channels: Used to read and write data over network sockets.
- Server Socket Channels: Used to listen for incoming TCP connections.

## 5. Input/Output (I/O):

### Console I/O:

Console I/O (Input/Output) facilitates reading from and writing to the console, enabling interaction with the user.

#### Types of Console I/O:

- Console I/O: Read and write data to the console.
- Console I/O (NIO.2): Read and write data to the console using NIO.2.
- Console I/O (Legacy): Read and write data to the console using legacy APIs.

#### Example:

```java
import java.io.Console;

public class ConsoleIOExample {
    public static void main(String[] args) {
        Console console = System.console();
        if (console != null) {
            String name = console.readLine("Enter your name: ");
            console.printf("Hello %s!", name);
        } else {
            System.out.println("Console not available!");
        }
    }
}
```

Output:

```java
Enter your name: John
Hello John!
```

### Network I/O:

Network I/O (Input/Output) involves reading from and writing to network connections for communication with other computers.

#### Types of Network I/O:

- Network I/O: Read and write data to network connections.
- Network I/O (NIO.2): Read and write data to network connections using NIO.2.
- Network I/O (Legacy): Read and write data to network connections using legacy APIs.
- Network I/O (Socket): Read and write data over network sockets.

#### Example:

```java
import java.net.*;
import java.io.*;

public class NetworkIOExample {
    public static void main(String[] args) {
        try (Socket socket = new Socket("localhost", 8080)) {
            BufferedReader br = new BufferedReader(new InputStreamReader(socket.getInputStream()));
            String line;
            while ((line = br.readLine()) != null) {
                System.out.println(line);
            }
        } catch (IOException e) {
            System.out.println("IOException caught!");
        }
    }
}
```

Output:

```java
Hello World!
```

These examples illustrate console I/O and network I/O operations, demonstrating interaction with the user via the console and reading from a network socket. The try-with-resources statement automatically closes resources after use.

### Standard I/O:

Standard I/O (Input/Output) is the process of reading from and writing to standard streams. It is used to interact with the user.

## 6. Concurrency:

Certainly! Let's organize and refine the provided information:

### Threads:

Threads are independent paths of execution within a program. They allow multiple tasks to be performed concurrently. Threads can be created by extending the Thread class or implementing the Runnable interface. They can be managed by the Thread class or the ExecutorService interface. Threads can be synchronized using locks or synchronized blocks. They can be made thread-safe by using the synchronized keyword or using thread-safe data structures.
Certainly! It seems like you've provided a list of statements about threads and their methods in Java. Let's organize and format it in a more readable way:

## Thread Communication:

- Threads can communicate using `wait()`, `notify()`, and `notifyAll()` methods.

## Thread Creation:

- Threads can be created using thread pools.

## Thread Interruption:

- Threads can be interrupted using the `interrupt()` method.

## Thread Joining:

- Threads can be joined using the `join()` method.

## Thread Daemonization:

- Threads can be set as daemon threads using the `setDaemon()` method.

## Thread Naming:

- Threads can be named using the `setName()` method.

## Thread Prioritization:

- Threads can be prioritized using the `setPriority()` method.

## Thread Suspension and Resumption:

- Threads can be suspended using the `suspend()` method.
- Threads can be resumed using the `resume()` method.

## Thread Stopping and Destruction (Deprecated):

- Threads can be stopped (deprecated) using the `stop()` method.
- Threads can be destroyed (deprecated) using the `destroy()` method.

## Thread Status:

- Threads can be checked for liveness using the `isAlive()` method.
- Threads can be checked for interrupted status using the `isInterrupted()` method.

## Thread Information Retrieval:

- Threads can be checked for daemon status using the `isDaemon()` method.
- Threads can be checked for name using the `getName()` method.
- Threads can be checked for priority using the `getPriority()` method.
- Threads can be checked for state using the `getState()` method.
- Threads can be checked for thread group using the `getThreadGroup()` method.
- Threads can be checked for thread ID using the `getId()` method.

## Other Thread Information Retrieval:

- Threads can be checked for stack trace elements using the `getStackTrace()` method.
- Threads can be checked for thread local variables using the `getThreadLocal()` method.
- Threads can be checked for context class loader using the `getContextClassLoader()` method.
- Threads can be checked for inherited access control context using the `getInheritedAccessControlContext()` method.

#### 1. Basic Thread Example:

thre

```java
public class ThreadExample {
    public static void main(String[] args) {
        // Creating and starting a new thread
        Thread thread = new Thread(() -> System.out.println("Hello World!"));
        thread.start();

        // Main thread continues its execution
        System.out.println("Main thread is still running.");
    }
}
```

Output:

```java
Main thread is still running.
Hello World!
```

In this example, a new thread is created to execute the task specified in the lambda expression concurrently with the main thread.

#### 2. Thread Synchronization Example:

thread synchronization is the process of ensuring that two or more concurrent threads do not simultaneously execute some particular program segment known as critical section. Critical section refers to the parts of the program where shared resource is accessed. For example, if a Java program has two threads, Thread A and Thread B, thread synchronization will ensure that operations in Thread A and Thread B are executed in a sequential manner. This will ensure that the values of shared objects are predictable, and the program will remain in a consistent state.

```java
public class ThreadSynchronizationExample {
    public static void main(String[] args) {
        // Creating a shared resource
        SharedResource sharedResource = new SharedResource();

        // Creating threads
        Thread thread1 = new Thread(() -> sharedResource.increment());
        Thread thread2 = new Thread(() -> sharedResource.decrement());

        // Starting threads
        thread1.start();
        thread2.start();
    }
}
```

output:

```java
0
1
```

In this example, two threads are created to increment and decrement a shared resource. Without synchronization, the output is unpredictable. With synchronization, the output is predictable.

#### 3. Thread Pools Example:

A thread pool is a collection of threads that can be reused to execute tasks. It is a container that contains a specified number of threads. It is used to reduce the overhead of creating new threads. It is also known as a thread executor.

```java
import java.util.concurrent.ExecutorService;
import java.util.concurrent.Executors;

public class ThreadPoolExample {
    public static void main(String[] args) {
        // Creating a thread pool with three threads
        ExecutorService executorService = Executors.newFixedThreadPool(3);

        // Submitting tasks to the thread pool
        for (int i = 0; i < 5; i++) {
            executorService.submit(() -> System.out.println("Task executed by thread: " + Thread.currentThread().getName()));
        }

        // Shutting down the thread pool
        executorService.shutdown();
    }
}
```

Output:

```java
Task executed by thread: pool-1-thread-1
Task executed by thread: pool-1-thread-3
Task executed by thread: pool-1-thread-2
Task executed by thread: pool-1-thread-1
Task executed by thread: pool-1-thread-2
```

In this example, a thread pool is created, and tasks are submitted to it. The thread pool efficiently manages the execution of tasks among its threads.

#### 4. Locks Example:

locks are used to sync locks types are reentrant lock, read write lock, stamped lock, condition lock, lock support, lock guard and lock support.

```java
import java.util.concurrent.locks.Lock;
import java.util.concurrent.locks.ReentrantLock;

public class LockExample {
    public static void main(String[] args) {
        // Creating a lock
        Lock lock = new ReentrantLock();

        // Creating a shared resource
        SharedResource sharedResource = new SharedResource();

        // Creating threads
        Thread thread1 = new Thread(() -> {
            lock.lock();
            try {
                sharedResource.increment();
            } finally {
                lock.unlock();
            }
        });
        Thread thread2 = new Thread(() -> {
            lock.lock();
            try {
                sharedResource.decrement();
            } finally {
                lock.unlock();
            }
        });

        // Starting threads
        thread1.start();
        thread2.start();
    }
}
```

#### 5. Thread Safety Example:

```java
public class ThreadSafetyExample {
    public static void main(String[] args) {
        // Creating a shared resource
        SharedResource sharedResource = new SharedResource();

        // Creating threads
        Thread thread1 = new Thread(() -> sharedResource.increment());
        Thread thread2 = new Thread(() -> sharedResource.decrement());

        // Starting threads
        thread1.start();
        thread2.start();
    }
}
```

#### 6. Thread Communication Example:

_Note: The "Thread Communication" example is a placeholder. If you have a specific scenario in mind for thread communication, please provide additional details, and I can help you create an example._

### 7. Additional Thread Pool Example:

```java
import java.util.concurrent.ExecutorService;
import java.util.concurrent.Executors;

public class AnotherThreadPoolExample {
    public static void main(String[] args) {
        // Creating a thread pool with 2 threads
        ExecutorService executor = Executors.newFixedThreadPool(2);

        // Submitting tasks for execution
        executor.submit(() -> System.out.println("Hello World!"));
        executor.submit(() -> System.out.println("Hello Java!"));

        // Shutting down the executor
        executor.shutdown();
    }
}
```

Output:

```java
Hello World!
Hello Java!
```

#### 8. Synchronization Example:

```java
public class SynchronizationExample {
    public static void main(String[] args) {
        // Creating a shared resource
        SharedResource sharedResource = new SharedResource();

        // Creating threads
        Thread thread1 = new Thread(() -> sharedResource.increment());
        Thread thread2 = new Thread(() -> sharedResource.decrement());

        // Starting threads
        thread1.start();
        thread2.start();
    }
}
```

#### 9. Locks Example with Explicit Lock:

```java
import java.util.concurrent.locks.Lock;
import java.util.concurrent.locks.ReentrantLock;

public class LockExample {
    public static void main(String[] args) {
        // Creating a lock
        Lock lock = new ReentrantLock();

        // Creating a shared resource
        SharedResource sharedResource = new SharedResource();

        // Creating threads
        Thread thread1 = new Thread(() -> {


 lock.lock();
            try {
                sharedResource.increment();
            } finally {
                lock.unlock();
            }
        });
        Thread thread2 = new Thread(() -> {
            lock.lock();
            try {
                sharedResource.decrement();
            } finally {
                lock.unlock();
            }
        });

        // Starting threads
        thread1.start();
        thread2.start();
    }
}
```

#### 10. Thread Safety Example (Repeated):

```java
public class ThreadSafetyExample {
    public static void main(String[] args) {
        // Creating a shared resource
        SharedResource sharedResource = new SharedResource();

        // Creating threads
        Thread thread1 = new Thread(() -> sharedResource.increment());
        Thread thread2 = new Thread(() -> sharedResource.decrement());

        // Starting threads
        thread1.start();
        thread2.start();
    }
}
```

#### 11. Thread Communication Example (Repeated):

```java
public class ThreadCommunicationExample {
    public static void main(String[] args) {
        // Creating a shared resource
        SharedResource sharedResource = new SharedResource();

        // Creating threads
        Thread thread1 = new Thread(() -> sharedResource.increment());
        Thread thread2 = new Thread(() -> sharedResource.decrement());

        // Starting threads
        thread1.start();
        thread2.start();
    }
}
```

#### 12. java database connectivity (JDBC) :

JDBC is an API for connecting Java applications with databases. It provides methods for querying and updating data in a database. It is used to interact with relational databases such as MySQL, Oracle, and SQL Server. It is also used to interact with non-relational databases such as MongoDB and Cassandra. JDBC is a part of the Java Standard Edition (Java SE) platform.

```java
import java.sql.*;

public class JDBCExample {
    public static void main(String[] args) {
        try {
            // Loading the JDBC driver
            Class.forName("com.mysql.cj.jdbc.Driver");

            // Creating a connection to the database
            Connection connection = DriverManager.getConnection("jdbc:mysql://localhost:3306/mydb", "root", "root");

            // Creating a statement
            Statement statement = connection.createStatement();

            // Executing a statement
            ResultSet resultSet = statement.executeQuery("SELECT * FROM users");

            // Iterating over the results
            while (resultSet.next()) {
                System.out.println(resultSet.getString("name"));
            }

            // Closing the connection
            connection.close();
        } catch (ClassNotFoundException e) {
            System.out.println("ClassNotFoundException caught!");
        } catch (SQLException e) {
            System.out.println("SQLException caught!");
        }
    }
}
```

Output:

```java
John
Jane
```

In this example, a connection is established with a MySQL database, and a query is executed to retrieve data from the `users` table.

#### 13. JDBC Transactions Example:

```java
import java.sql.*;

public class JDBCTransactionsExample {
    public static void main(String[] args) {
        try {
            // Loading the JDBC driver
            Class.forName("com.mysql.cj.jdbc.Driver");

            // Creating a connection to the database
            Connection connection = DriverManager.getConnection("jdbc:mysql://localhost:3306/mydb", "root", "root");

            // Turning off auto-commit mode
            connection.setAutoCommit(false);

            // Creating a statement
            Statement statement = connection.createStatement();

            // Executing a statement
            statement.executeUpdate("INSERT INTO users (name) VALUES ('John')");

            // Committing the transaction
            connection.commit();

            // Closing the connection
            connection.close();
        } catch (ClassNotFoundException e) {
            System.out.println("ClassNotFoundException caught!");
        } catch (SQLException e) {
            System.out.println("SQLException caught!");
        }
    }
}
```

In this example, a connection is established with a MySQL database, and a transaction is executed to insert data into the `users` table.

#### 14. JDBC Batch Processing Example:

```java
import java.sql.*;

public class JDBCBatchProcessingExample {
    public static void main(String[] args) {
        try {
            // Loading the JDBC driver
            Class.forName("com.mysql.cj.jdbc.Driver");

            // Creating a connection to the database
            Connection connection = DriverManager.getConnection("jdbc:mysql://localhost:3306/mydb", "root", "root");

            // Turning off auto-commit mode
            connection.setAutoCommit(false);

            // Creating a statement
            Statement statement = connection.createStatement();

            // Adding statements to the batch
            statement.addBatch("INSERT INTO users (name) VALUES ('John')");
            statement.addBatch("INSERT INTO users (name) VALUES ('Jane')");

            // Executing the batch
            statement.executeBatch();

            // Committing the transaction
            connection.commit();

            // Closing the connection
            connection.close();
        } catch (ClassNotFoundException e) {
            System.out.println("ClassNotFoundException caught!");
        } catch (SQLException e) {
            System.out.println("SQLException caught!");
        }
    }
}
```

In this example, a connection is established with a MySQL database, and a batch of statements is executed to insert data into the `users` table.

#### 15. JDBC Prepared Statements Example:

```java
import java.sql.*;

public class JDBCPreparedStatementsExample {
    public static void main(String[] args) {
        try {
            // Loading the JDBC driver
            Class.forName("com.mysql.cj.jdbc.Driver");

            // Creating a connection to the database
            Connection connection = DriverManager.getConnection("jdbc:mysql://localhost:3306/mydb", "root", "root");

            // Creating a prepared statement
            PreparedStatement preparedStatement = connection.prepareStatement("INSERT INTO users (name) VALUES (?)");

            // Setting parameters
            preparedStatement.setString(1, "John");

            // Executing the statement
            preparedStatement.executeUpdate();

            // Closing the connection
            connection.close();
        } catch (ClassNotFoundException e) {
            System.out.println("ClassNotFoundException caught!");
        } catch (SQLException e) {
            System.out.println("SQLException caught!");
        }
    }
}
```

In this example, a connection is established with a MySQL database, and a prepared statement is executed to insert data into the `users` table.

#### 16. JDBC Stored Procedures Example:

```java
import java.sql.*;

public class JDBCStoredProceduresExample {
    public static void main(String[] args) {
        try {
            // Loading the JDBC driver
            Class.forName("com.mysql.cj.jdbc.Driver");

            // Creating a connection to the database
            Connection connection = DriverManager.getConnection("jdbc:mysql://localhost:3306/mydb", "root", "root");

            // Creating a callable statement
            CallableStatement callableStatement = connection.prepareCall("{CALL get_users()}");

            // Executing the statement
            ResultSet resultSet = callableStatement.executeQuery();

            // Iterating over the results
            while (resultSet.next()) {
                System.out.println(resultSet.getString("name"));
            }

            // Closing the connection
            connection.close();
        } catch (ClassNotFoundException e) {
            System.out.println("ClassNotFoundException caught!");
        } catch (SQLException e) {
            System.out.println("SQLException caught!");
        }
    }
}
```

In this example, a connection is established with a MySQL database, and a stored procedure is executed to retrieve data from the `users` table.

#### java beans :

JavaBeans are reusable software components for Java. They are classes that encapsulate many objects into a single object (the bean). They are serializable, have a zero-argument constructor, and allow access to properties using getter and setter methods. They are used to simplify the development of large applications. They are also used to encapsulate data and functionality into a single unit. They are a part of the Java Standard Edition (Java SE) platform.

```java
public class JavaBeansExample {
    private String name;
    private int age;

    public JavaBeansExample() {
    }

    public JavaBeansExample(String name, int age) {
        this.name = name;
        this.age = age;
    }

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public int getAge() {
        return age;
    }

    public void setAge(int age) {
        this.age = age;
    }
}
```

In this example, a JavaBean is created to encapsulate data and functionality into a single unit.

Certainly! Let's format the information into clear and concise sections:

## **Java Reflection:**

- **Definition:**
  Reflection is the process of examining or modifying the behavior of a program at runtime. It allows inspection, analysis, and modification of classes, interfaces, and methods dynamically.

- **Usage:**
  - Used to instantiate classes, invoke methods, and access fields.
  - Implements dependency injection frameworks like Spring and object-relational mapping (ORM) frameworks such as Hibernate.
  - Part of the Java Standard Edition (Java SE) platform.

- **Example:**
  ```java
  import java.lang.reflect.Constructor;
  import java.lang.reflect.Field;
  import java.lang.reflect.Method;

  public class JavaReflectionExample {
      public static void main(String[] args) {
          try {
              // Getting the class object
              Class<?> clazz = Class.forName("java.lang.String");

              // Getting the constructors
              Constructor<?>[] constructors = clazz.getConstructors();

              // Getting the fields
              Field[] fields = clazz.getFields();

              // Getting the methods
              Method[] methods = clazz.getMethods();
          } catch (ClassNotFoundException e) {
              System.out.println("ClassNotFoundException caught!");
          }
      }
  }
  ```

## **Java Annotations:**

- **Definition:**
  Annotations provide metadata about a program without modifying the code itself. They offer instructions to the compiler, runtime environment, build tools, IDE, and more.

- **Usage:**
  - Applied at various levels, such as source code generation, unit testing, and deployment.
  - Used for providing instructions to different tools like monitoring, logging, security, etc.

- **Example:**
  ```java
  import java.lang.annotation.*;

  @Retention(RetentionPolicy.RUNTIME)
  @Target(ElementType.TYPE)
  @interface MyAnnotation {
      String value();
  }

  @MyAnnotation("Hello World!")
  public class JavaAnnotationsExample {
      public static void main(String[] args) {
          // Getting the class object
          Class<?> clazz = JavaAnnotationsExample.class;

          // Getting the annotation
          MyAnnotation myAnnotation = clazz.getAnnotation(MyAnnotation.class);

          // Printing the annotation value
          System.out.println(myAnnotation.value());
      }
  }
  ```

## **Java Generics:**

- **Definition:**
  Generics provide compile-time type safety for various Java elements.

- **Usage:**
  - Ensures type safety for collections, classes, methods, interfaces, etc.

- **Example:**
  ```java
  import java.util.ArrayList;
  import java.util.List;

  public class JavaGenericsExample {
      public static void main(String[] args) {
          // Creating a list of integers
          List<Integer> numbers = new ArrayList<>();

          // Adding elements to the list
          numbers.add(1);
          numbers.add(2);
          numbers.add(3);

          // Iterating over the list
          for (int i : numbers) {
              System.out.println(i);
          }
      }
  }
  ```

## **Java Streams:**

- **Definition:**
  Streams are used for performing operations on collections.

- **Usage:**
  - Applicable to arrays, files, I/O, networking, concurrency, JDBC, JavaBeans, reflection, and annotations.

- **Example:**
  ```java
  import java.util.ArrayList;
  import java.util.List;

  public class JavaStreamsExample {
      public static void main(String[] args) {
          // Creating a list of integers
          List<Integer> numbers = new ArrayList<>();

          // Adding elements to the list
          numbers.add(1);
          numbers.add(2);
          numbers.add(3);

          // Iterating over the list
          numbers.stream().forEach(System.out::println);
      }
  }
  ```

## **Java I/O:**

- **Definition:**
  I/O (Input/Output) is the process of reading from and writing to files. It is used for persistent data storage and interaction with various elements.

- **Usage:**
  - Essential for persistent data storage, user interaction, networking, etc.
  - Interacts with console, network, database, JavaBeans, reflection, annotations, and streams.

- **Example:**
  ```java
  import java.io.*;

  public class JavaIOExample {
      public static void main(String[] args) {
          try (BufferedReader reader = new BufferedReader(new FileReader("input.txt"));
               BufferedWriter writer = new BufferedWriter(new FileWriter("output.txt"))) {
              String line;
              while ((line = reader.readLine()) != null) {
                  writer.write(line);
                  writer.newLine();
              }
          } catch (IOException e) {
              System.out.println("IOException caught!");
          }
      }
  }
  ```
---
END OF FILE 
--