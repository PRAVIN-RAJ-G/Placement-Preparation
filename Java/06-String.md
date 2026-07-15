
# ☕ Strings in Java

## What is a String?

A String is a sequence of characters used to store text.

### Example

```java
String name = "Pravin";
```

Here,

- `String` → Data Type
- `name` → Variable
- `"Pravin"` → String Value

---

# Creating a String

Strings can be created in two ways:

1. Using String Literal
2. Using `new` Keyword

---

## 1. Using String Literal

```java
String name = "Java";
```

---

## 2. Using `new` Keyword

```java
String name = new String("Java");
```

---

# String is Immutable

In Java, Strings are **immutable**.

Immutable means once a String object is created, its original value cannot be changed.

### Example

```java
String name = "Java";
name = name + " Programming";

System.out.println(name);
```

The original `"Java"` String is not modified. A new String object is created.

---

# String Methods

Java provides several built-in methods to perform operations on Strings.

---

## length()

Returns the number of characters in a String.

```java
String name = "Java";

System.out.println(name.length());
```

### Output

```text
4
```

---

## charAt()

Returns the character at a specified index.

```java
String name = "Java";

System.out.println(name.charAt(0));
```

### Output

```text
J
```

---

## toUpperCase()

Converts all characters into uppercase.

```java
String name = "java";

System.out.println(name.toUpperCase());
```

### Output

```text
JAVA
```

---

## toLowerCase()

Converts all characters into lowercase.

```java
String name = "JAVA";

System.out.println(name.toLowerCase());
```

### Output

```text
java
```

---

## equals()

Compares the content of two Strings.

```java
String a = "Java";
String b = "Java";

System.out.println(a.equals(b));
```

### Output

```text
true
```

---

## equalsIgnoreCase()

Compares two Strings without considering uppercase and lowercase differences.

```java
String a = "Java";
String b = "JAVA";

System.out.println(a.equalsIgnoreCase(b));
```

### Output

```text
true
```

---

## contains()

Checks whether a String contains a particular sequence of characters.

```java
String text = "Java Programming";

System.out.println(text.contains("Java"));
```

### Output

```text
true
```

---

## substring()

Extracts a part of a String.

```java
String text = "Java Programming";

System.out.println(text.substring(0, 4));
```

### Output

```text
Java
```

---

## replace()

Replaces a character or sequence of characters.

```java
String text = "Java";

System.out.println(text.replace('a', 'o'));
```

### Output

```text
Jovo
```

---

## trim()

Removes spaces from the beginning and end of a String.

```java
String text = "  Java  ";

System.out.println(text.trim());
```

---

# Comparing Strings

## Using `==`

The `==` operator compares the references of String objects.

## Using `equals()`

The `equals()` method compares the actual content of Strings.

### Example

```java
String a = new String("Java");
String b = new String("Java");

System.out.println(a == b);
System.out.println(a.equals(b));
```

### Output

```text
false
true
```

---

# String Concatenation

String concatenation means joining two or more Strings.

### Using `+`

```java
String firstName = "Pravin";
String lastName = "Raj";

String fullName = firstName + " " + lastName;

System.out.println(fullName);
```

### Output

```text
Pravin Raj
```

---


# StringBuilder and StringBuffer

Since `String` is immutable, `StringBuilder` and `StringBuffer` are used when we need to modify a String multiple times.

## StringBuilder

`StringBuilder` is mutable, which means its content can be changed.

It is faster but not thread-safe.

### Example

```java
StringBuilder name = new StringBuilder("Java");

name.append(" Programming");

System.out.println(name);
```

### Output

```text
Java Programming
```

---

## StringBuffer

`StringBuffer` is also mutable.

It is thread-safe but slower than `StringBuilder`.

### Example

```java
StringBuffer name = new StringBuffer("Java");

name.append(" Programming");

System.out.println(name);
```

### Output

```text
Java Programming
```

---

## Difference

| String | StringBuilder | StringBuffer |
|---|---|---|
| Immutable | Mutable | Mutable |
| Cannot modify the original object | Can modify the same object | Can modify the same object |
| — | Faster | Slower |
| — | Not thread-safe | Thread-safe |

---

# Quick Revision

- String → Sequence of characters.
- String is a non-primitive data type.
- String objects are immutable.
- `length()` → Returns the number of characters.
- `charAt()` → Returns a character at a particular index.
- `==` → Compares references.
- `equals()` → Compares content.
- `+` → Used for String concatenation.

---
