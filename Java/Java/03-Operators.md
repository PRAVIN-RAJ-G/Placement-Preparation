# ☕ Operators in Java

## What is an Operator?

An operator is a special symbol used to perform operations on one or more operands (values or variables).

### Example

```java
int a = 10;
int b = 5;

int c = a + b;
```

Here,

- `+` → Operator
- `a` and `b` → Operands

---

# Types of Operators in Java

There are **6 types of operators** in Java.

1. Arithmetic Operators
2. Relational Operators
3. Logical Operators
4. Assignment Operators
5. Unary Operators
6. Ternary Operator

---

# 1. Arithmetic Operators

Arithmetic operators are used to perform mathematical operations.

| Operator | Meaning |
|----------|---------|
| + | Addition |
| - | Subtraction |
| * | Multiplication |
| / | Division |
| % | Modulus (Remainder) |

### Example

```java
int a = 20;
int b = 10;

System.out.println(a + b);

---

# 2. Relational Operators

Relational operators are used to compare two values.

The result will always be **true** or **false**.

| Operator | Meaning |
|----------|---------|
| == | Equal to |
| != | Not Equal to |
| > | Greater than |
| < | Less than |
| >= | Greater than or Equal to |
| <= | Less than or Equal to |

### Example

```java
int a = 20;
int b = 10;

System.out.println(a > b);
System.out.println(a == b);
```

---

# 3. Logical Operators

Logical operators are used to combine two or more conditions.

| Operator | Meaning |
|----------|---------|
| && | Logical AND |
| \|\| | Logical OR |
| ! | Logical NOT |

### Example

```java
int age = 22;

System.out.println(age > 18 && age < 60);
```

---

# 4. Assignment Operators

Assignment operators are used to assign values to variables.

| Operator | Meaning |
|----------|---------|
| = | Assign |
| += | Add and Assign |
| -= | Subtract and Assign |
| *= | Multiply and Assign |
| /= | Divide and Assign |
| %= | Modulus and Assign |

### Example

```java
int a = 10;

a += 5;

System.out.println(a);
```

---

# 5. Unary Operators

Unary operators work on a single operand.

| Operator | Meaning |
|----------|---------|
| ++ | Increment |
| -- | Decrement |
| + | Unary Plus |
| - | Unary Minus |
| ! | Logical NOT |

### Example

```java
int a = 10;

a++;

System.out.println(a);
```

---

# 6. Ternary Operator

The ternary operator is used as a shortcut for the if-else statement.

### Syntax

```java
condition ? true_value : false_value;
```

### Example

```java
int age = 18;

String result = (age >= 18) ? "Eligible" : "Not Eligible";

System.out.println(result);
```

---

# Quick Revision

- Operator → Performs an operation.
- Operand → Value on which the operation is performed.
- Arithmetic → Mathematical operations.
- Relational → Comparison (True/False).
- Logical → Combines conditions.
- Assignment → Assigns values.
- Unary → Works with one operand.
- Ternary → Short form of if-else.

---
