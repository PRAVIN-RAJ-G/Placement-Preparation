
# Object-Oriented Programming (OOP) in Java

## What is Object-Oriented Programming?

**Object-Oriented Programming (OOP)** is a programming approach where programs are designed using **objects and classes**.

### Four Major Components of OOP

1. **Encapsulation**
2. **Inheritance**
3. **Polymorphism**
4. **Abstraction**

---

# 1. Encapsulation

### Definition

> The process of **binding data (state) and behaviour (methods) together** into a single unit is called **Encapsulation**.

In Java, a **class** is an example of encapsulation because it contains variables and methods together.

### Major Advantage

The major advantage of encapsulation is **Data Hiding**.

### Data Hiding

> The process of restricting direct access to data and providing controlled access through methods is called **Data Hiding**.

We can achieve data hiding using the **`private` access modifier**.

### Example

```java
class Student {

    private int marks;

    public void setMarks(int marks) {
        this.marks = marks;
    }

    public int getMarks() {
        return marks;
    }
}
```

Here:

* `marks` → private data
* `setMarks()` → setter method
* `getMarks()` → getter method

So, the data cannot be accessed directly from outside the class.

---

# 2. Inheritance

### Definition

> The process of acquiring the **properties and behaviours of one class into another class** is called **Inheritance**.

### Major Advantage

The major advantage of inheritance is **Code Reusability**.

### How to achieve Inheritance?

In Java, inheritance can be achieved using:

1. `extends`
2. `implements`

### Example using `extends`

```java
class Parent {
    void display() {
        System.out.println("Parent");
    }
}

class Child extends Parent {
}
```

Here, `Child` inherits the `display()` method from `Parent`.

---

## Types of Inheritance

1. **Single Level Inheritance**
2. **Multilevel Inheritance**
3. **Hierarchical Inheritance**
4. **Multiple Inheritance**
5. **Hybrid Inheritance**

> **Important:** Multiple inheritance is **not supported through classes in Java** because it can create ambiguity.

Multiple inheritance can be achieved in Java using **interfaces**.

---

## `super` Keyword

The `super` keyword is used to refer to the **parent class**.

### Super Constructor

`super()` is used to call the **parent class constructor** from the child class constructor.

```java
class Parent {

    Parent() {
        System.out.println("Parent Constructor");
    }
}

class Child extends Parent {

    Child() {
        super();
        System.out.println("Child Constructor");
    }
}
```

### Important Point

`super()` must be the **first statement** inside the child constructor.

---

# 3. Polymorphism

### Definition

> **Polymorphism** means **one name having many forms**.

The word polymorphism is derived from:

* **Poly** → Many
* **Morph** → Forms

### Types of Polymorphism

1. **Compile-Time Polymorphism**

   * Method Overloading

2. **Run-Time Polymorphism**

   * Method Overriding

---

## Compile-Time Polymorphism

### Method Overloading

> Having **multiple methods with the same name but different formal arguments** is called Method Overloading.

### Example

```java
class Calculator {

    void add(int a, int b) {
        System.out.println(a + b);
    }

    void add(int a, int b, int c) {
        System.out.println(a + b + c);
    }
}
```

Here, both methods have the same name `add()` but different parameters.

Therefore, it is **Method Overloading**.

### Method Overloading can differ by:

* Number of parameters
* Type of parameters
* Order of parameters

> **Return type alone cannot be used for method overloading.**

---

# Run-Time Polymorphism

## Method Overriding

> The process of **changing/redefining the implementation of a method in the child class which is already present in the parent class** is called Method Overriding.

### Example

```java
class Parent {

    void display() {
        System.out.println("Parent");
    }
}

class Child extends Parent {

    @Override
    void display() {
        System.out.println("Child");
    }
}
```

Here, the `display()` method is already present in the parent class and its implementation is changed in the child class.

Therefore, it is **Method Overriding**.

### Important Point

Method overriding is associated with **inheritance** and is used to achieve **Run-Time Polymorphism**.

---

# 4. Abstraction

### Definition

> The process of **hiding implementation details and providing only the necessary features to the user** is called Abstraction.

### Example

When we use an ATM, we only interact with options such as:

* Withdraw
* Deposit
* Check Balance

We don't need to know the internal implementation of the banking system.

That is **Abstraction**.

---

# Abstract Method

> A method which **does not have a method body** is called an **Abstract Method**.

### Syntax

```java
abstract void display();
```

---

# Concrete Method

> A method which **has a method body** is called a **Concrete Method**.

### Example

```java
void display() {
    System.out.println("Hello");
}
```

---

# Abstract Class

> A class declared using the `abstract` keyword is called an **Abstract Class**.

An abstract class can contain:

* Abstract methods
* Concrete methods
* Variables
* Constructors

### Example

```java
abstract class WhatsApp {

    abstract void createGroup();

    void chat() {
        System.out.println("Hi from chat");
    }
}
```

Here:

* `createGroup()` → Abstract method
* `chat()` → Concrete method

### Important Point

An abstract class can provide **both abstraction and implementation**.

---

# Interface

### Definition

> An interface is a Java component similar to a class that is mainly used to achieve **abstraction** and define a contract for implementing classes.

### Important Points

* An interface does not have a constructor.
* We cannot create an object directly for an interface.
* A class uses `implements` to implement an interface.
* An interface can extend another interface.
* A class cannot extend an interface.

### Example

```java
interface Animal {

    void sound();
}

class Dog implements Animal {

    public void sound() {
        System.out.println("Dog barks");
    }
}
```

---

# `extends` vs `implements`

| Keyword      | Used With             |
| ------------ | --------------------- |
| `extends`    | Class → Class         |
| `extends`    | Interface → Interface |
| `implements` | Class → Interface     |

### Remember

```java
class Child extends Parent
```

```java
class Dog implements Animal
```

```java
interface ChildInterface extends ParentInterface
```

### Important

Multiple inheritance is **not possible with classes**:

```text
Class A       Class B
    \           /
     \         /
       Class C
       ❌ Not possible
```

But multiple inheritance is possible using interfaces:

```text
Interface A     Interface B
      \           /
       \         /
         Class C
       implements
      both interfaces
```

---

# Formal Argument

> The variable which accepts the incoming value during method declaration is called a **Formal Argument** (Formal Parameter).

### Example

```java
void add(int a, int b)
```

Here:

* `a` → Formal argument
* `b` → Formal argument

---

# Actual Argument

> The value which is provided to the formal argument during a method call is called an **Actual Argument**.

### Example

```java
add(10, 20);
```

Here:

* `10` → Actual argument
* `20` → Actual argument

### Easy Difference

```java
void add(int a, int b)   // Formal arguments

add(10, 20);             // Actual arguments
```

---

# Method Signature

> The **method name along with its formal parameter list** is called the **Method Signature**.

### Example

```java
void add(int a, int b)
```

Method signature:

```text
add(int, int)
```

> Return type is **not part of the method signature** in Java.

---

# Access Modifiers

### Definition

> Access modifiers define the **accessibility and visibility** of a class member.

Access modifiers can be used with:

* Variables
* Methods
* Constructors
* Classes (where applicable)

### Types of Access Modifiers

1. `public`
2. `private`
3. `default`
4. `protected`

---

## 1. Public

A `public` member can be accessed from **anywhere**, subject to normal class/package access rules.

```java
public int marks;
```

---

## 2. Private

A `private` member can be accessed **only within the same class**.

```java
private int marks;
```

It is mainly used to achieve **data hiding**.

---

## 3. Default

When no access modifier is specified, it is called **default access**.

```java
int marks;
```

It can be accessed within the **same package**.

---

## 4. Protected

A `protected` member can be accessed:

* Within the same package
* In a child class, including a child class in another package through inheritance

```java
protected int marks;
```

---

# Quick OOP Revision

| OOP Concept       | Main Purpose                  |
| ----------------- | ----------------------------- |
| **Encapsulation** | Binding data + methods        |
| **Data Hiding**   | Restricting direct access     |
| **Inheritance**   | Code reusability              |
| **Polymorphism**  | One name, many forms          |
| **Abstraction**   | Hiding implementation details |

### Polymorphism

```text
Compile-Time  → Method Overloading
Run-Time      → Method Overriding
```

### Abstraction

```text
Abstract Class → Can contain abstract + concrete methods
Interface      → Used to define a contract / achieve abstraction
```

### Inheritance

```text
Class → Class       → extends
Class → Interface   → implements
Interface → Interface → extends
```
