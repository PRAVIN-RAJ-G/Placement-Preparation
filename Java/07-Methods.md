# ☕ Methods in Java

## What is a Method?

A method is a block of code used to perform a specific task.

A method executes only when it is called.

### Example

```java
static void greet()
{
    System.out.println("Hello");
}
```

To execute the method:

```java
greet();
```

---

# Why do we use Methods?

Methods are used to:

- Avoid code repetition.
- Reuse the same code multiple times.
- Divide a large program into smaller parts.
- Make the program easier to understand.
- Make the code easier to maintain.

### Without Method

```java
System.out.println("Welcome to Java");
System.out.println("Welcome to Java");
System.out.println("Welcome to Java");
```

### With Method

```java
static void welcome()
{
    System.out.println("Welcome to Java");
}

public static void main(String[] args)
{
    welcome();
    welcome();
    welcome();
}
```

Here, the same method can be called multiple times without writing the same code again.

---

# Method Syntax

## Syntax

```java
[Access Modifier] [Modifier] ReturnType MethodName(Formal Arguments)
{
    // Instructions
}
```

### Example

```java
public static void main(String[] args)
{
    System.out.println("Hello World");
}
```

### Explanation

- **public** → Access Modifier
- **static** → Modifier
- **void** → Return Type
- **main** → Method Name
- **String[] args** → Formal Arguments

---

# Access Modifier

An Access Modifier decides the visibility and accessibility of a method or variable.

It is written as a prefix before the method declaration.

## Types of Access Modifiers

- **public** – Accessible from anywhere.
- **private** – Accessible only within the same class.
- **default** – Accessible only within the same package.
- **protected** – Accessible within the same package and also outside the package through inheritance.

---

# Modifier

A modifier changes the behavior of a method.

### Common Modifier

- **static** – Allows the method to be called without creating an object.

Example:

```java
public static void display()
{
    System.out.println("Java");
}
```

---

# Return Type

The return type specifies what type of value a method returns after execution.

### Common Return Types

- `void` → Returns nothing.
- `int` → Returns an integer.
- `double` → Returns a decimal value.
- `char` → Returns a character.
- `boolean` → Returns true or false.
- `String` → Returns a string.

Example

```java
int add()
{
    return 10;
}
```

---

# Method Signature

Method Name + Formal Arguments is called the **Method Signature**.

Example

```java
sum(int a, int b)
```

Here,

- Method Name → `sum`
- Formal Arguments → `(int a, int b)`

Method Signature:

```java
sum(int a, int b)
```

---

# Types of Methods

Methods are classified into two types.

1. Parameterized Method
2. Non-Parameterized Method

---

# Parameterized Method

A method that accepts one or more parameters (formal arguments) is called a **Parameterized Method**.

### Example

```java
static void add(int a, int b)
{
    System.out.println(a + b);
}
```

Calling

```java
add(10,20);
```

---

# Non-Parameterized Method

A method that does not accept any parameters is called a **Non-Parameterized Method**.

### Example

```java
static void display()
{
    System.out.println("Welcome");
}
```

Calling

```java
display();
```

---

# Formal Argument

The variables declared in the method definition to receive values are called **Formal Arguments**.

Example

```java
static void add(int a, int b)
{
}
```

Here,

- `a`
- `b`

are Formal Arguments.

---

# Actual Argument

The values passed while calling a method are called **Actual Arguments**.

Example

```java
add(10,20);
```

Here,

- `10`
- `20`

are Actual Arguments.

---
