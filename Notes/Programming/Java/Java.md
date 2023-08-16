##### Description
This is a Java Guide based on Platzi, W3schools, and Geeksforgeeks.
##### Sources:
- [Platzi](https://platzi.com/ruta/web-java/)
- [W3Schools](https://www.w3schools.com/java/)
- [GeeksforGeeks](https://www.geeksforgeeks.org/java/)
.

## Fundamentals
##### Datatypes
Java's Primitive Datatypes are:

![[Pasted image 20230809132908.png]]
- Strings are not a Primitive Datatype but a Class in Java.
.

##### Conditionals
- `if/else`
```java
if (condition1) {
  // block of code to be executed if condition1 is true
} else if (condition2) {
  // block of code to be executed if the condition1 is false and condition2 is true
} else {
  // block of code to be executed if the condition1 is false and condition2 is false
}
```
- Java `if/else` can be written in a shorthand way;
```java
variable = (condition) ? expressionTrue :  expressionFalse;
```

- Instead of writing many if/else statements, you can use the `switch` statement.
```java
switch(expression) {
  case x:
    // code block
    break;
  case y:
    // code block
    break;
  default:
    // code block
}
```
.

##### Loops
- `while` loops
```java
while (condition) {
  // code block to be executed
}
```

- `for` loops
```java
for (statement 1; statement 2; statement 3) {
  // code block to be executed
}
```
.
.

## Collections
##### Array
- Arrays are used to store multiple values in a single variable, instead of declaring separate variables for each value.

```java
String[] cars = {"Volvo", "BMW", "Ford", "Mazda"};
```
.

##### Lists (ArrayList)
- The `ArrayList` class is a resizable array, which can be found in the `java.util` package.
- The difference between a built-in array and an `ArrayList` in Java, is that the size of an array cannot be modified (if you want to add or remove elements to/from an array, you have to create a new one). While elements can be added and removed from an `ArrayList` whenever you want.

```java
import java.util.ArrayList; // import the ArrayList class

ArrayList<String> cars = new ArrayList<String>(); // Create an ArrayList object
```

- You can add
```java
 cars.add("Volvo");
```
- Access
```java
cars.get(0);
```
- Change a value
```java
cars.set(0, "Opel");
```
- Remove an item
```java
cars.remove(0);
```
- Remove all ArrayList elements
```java
cars.clear();
```
- Check the ArrayList size
```java
cars.size();
```
.

##### Linked Lists
- The `LinkedList` class is a collection which can contain many objects of the same type, just like the `ArrayList`.
```java
 LinkedList<String> cars = new LinkedList<String>();
    cars.add("Volvo");
    cars.add("BMW");
    cars.add("Ford");
    cars.add("Mazda");
    System.out.println(cars);
```
- The `LinkedList` stores its items in "containers." The list has a link to the first container and each container has a link to the next container in the list. To add an element to the list, the element is placed into a new container and that container is linked to one of the other containers in the list.
- For many cases, the `ArrayList` is more efficient as it is common to need access to random items in the list, but the `LinkedList` provides several methods to do certain operations more efficiently;
	- addFirst(), addLast(), removeFirst(), removeLast(), getFirst(), getLast()
.

##### Queue

.
##### Stacks

.

##### Maps

.

##### Trees

.
.

## Object Oriented Programming
##### Basics
- Everything in Java is associated with classes and objects, along with its attributes and methods.
- A `Class` is like an object constructor, or a "blueprint" for creating objects.
- `attributes` are characteristics of the class
- `methods` are actions of the class (in the form of functions)
.

##### Constructors
- A constructor in Java is a **special method** that is used to initialize objects. The constructor is called when an object of a class is created.
- Constructors can also take parameters, which is used to initialize attributes.
.

##### Modifiers
We divide modifiers into two groups:
- **Access Modifiers** - controls the access level
- **Non-Access Modifiers** - do not control access level, but provides other functionality
.
![[Pasted image 20230810121552.png]]
.
![[Pasted image 20230810121615.png]]
.

#### Object Oriented Principles
##### Encapsulation
The meaning of **Encapsulation**, is to make sure that "sensitive" data is hidden from users. To achieve this, you must:

- declare class variables/attributes as `private`
- provide public **get** and **set** methods to access and update the value of a `private` variable
```java
public class Person {
  private String name; // private = restricted access

  // Getter
  public String getName() {
    return name;
  }

  // Setter
  public void setName(String newName) {
    this.name = newName;
  }
}
```
.
##### Inheritance
In Java, it is possible to inherit attributes and methods from one class to another. We group the "inheritance concept" into two categories:

- **subclass** (child) - the class that inherits from another class
- **superclass** (parent) - the class being inherited from

To inherit from a class, use the `extends` keyword.
```java
class Vehicle {
  protected String brand = "Ford";        // Vehicle attribute
  public void honk() {                    // Vehicle method
    System.out.println("Tuut, tuut!");
  }
}

class Car extends Vehicle {
  private String modelName = "Mustang";    // Car attribute
  public static void main(String[] args) {

    // Create a myCar object
    Car myCar = new Car();

    // Call the honk() method (from the Vehicle class) on the myCar object
    myCar.honk();

    // Display the value of the brand attribute (from the Vehicle class) and the value of the modelName from the Car class
    System.out.println(myCar.brand + " " + myCar.modelName);
  }
}
```

- If you don't want other classes to inherit from a class, use the `final`
.

##### Polymorphism
- Its the ability to change the behaviors (methods) of a subclass.
.

##### Abstraction

.
.

## SOLID Principles


.
.

## Test Driven Development

.
.


## Miscellaneous
##### Input/Output

.

##### Environment

.

##### JVM, JRE, JIT, and JDK

.

##### Packages
A package in Java is used to group related classes. Think of it as **a folder in a file directory**. We use packages to avoid name conflicts, and to write a better maintainable code. Packages are divided into two categories:

- **Built-in Packages** (packages from the Java API)
- **User-defined Packages** (create your own packages)
.
##### Built-in Packages
The Java API is a library of prewritten classes, that are free to use, included in the Java Development Environment.

The library contains components for managing input, database programming, and much much more. The complete list can be found at Oracles website: [https://docs.oracle.com/javase/8/docs/api/](https://docs.oracle.com/javase/8/docs/api/).

The library is divided into **packages** and **classes**. Meaning you can either import a single class (along with its methods and attributes), or a whole package that contain all the classes that belong to the specified package.
```java
import package.name.Class;   // Import a single class
import package.name.*;   // Import the whole package
```
.
##### User-defined Packages
To create your own package, you need to understand that Java uses a file system directory to store them. Just like folders on your computer:
└── root
  └── mypack
    └── MyPackageClass.java

To create a package, use the `package` keyword:
```java
package mypack;
class MyPackageClass {
  public static void main(String[] args) {
    System.out.println("This is my package!");
  }
}
```
.

##### Javadocs

.

##### Maven

.

##### Linter
[Checkstyle](https://github.com/checkstyle/checkstyle)

.
.


.
And finally... ****[[Spring]]****

:)
.