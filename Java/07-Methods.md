
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

Methods are mainly used to:

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

### Syntax

```java
returnType methodName(parameters)
{
    // method body
}
```

### Example

```java
static void display()
{
    System.out.println("Java");
}
```

### Explanation

- `static` → Allows the method to be called directly from the `main` method.
- `void` → The method does not return any value.
- `display` → Method name.
- `()` → Used to pass parameters.
- `{ }` → Contains the method body.

### Calling the Method

```java
display();
```

A method must be called to execute the code inside it.

---
