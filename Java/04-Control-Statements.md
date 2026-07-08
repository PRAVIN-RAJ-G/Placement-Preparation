# ☕ Control Statements in Java

## What is a Control Statement?

A control statement is used to control the flow of program execution based on a condition or repetition.

---

# Types of Control Statements

There are three types of control statements.

1. Conditional Statements
2. Iteration (Looping) Statements
3. Jump Statements

---

# 1. Selection Statements

Selection statements are used to execute a block of code based on a condition.

Types of Selection Statements

- if
- if-else
- else-if
- nested if
- switch

---

## if Statement

The `if` statement executes a block of code only if the given condition is **true**.

### Syntax

```java
if(condition)
{
    // statements
}
```

### Example

```java
int age = 20;

if(age >= 18)
{
    System.out.println("Eligible to Vote");
}
```

---

## if-else Statement

The `if-else` statement executes one block if the condition is true; otherwise, it executes another block.

### Syntax

```java
if(condition)
{
    // statements
}
else
{
    // statements
}
```

### Example

```java
int age = 16;

if(age >= 18)
{
    System.out.println("Eligible");
}
else
{
    System.out.println("Not Eligible");
}
```

---

## else-if Ladder

The `else-if` ladder is used to check multiple conditions.

### Example

```java
int mark = 85;

if(mark >= 90)
{
    System.out.println("Grade A");
}
else if(mark >= 75)
{
    System.out.println("Grade B");
}
else
{
    System.out.println("Grade C");
}
```

---

## Nested if

A nested if means an `if` statement inside another `if` statement.

### Example

```java
int age = 20;
boolean idCard = true;

if(age >= 18)
{
    if(idCard)
    {
        System.out.println("Allowed");
    }
}
```

---

## switch Statement

The `switch` statement is used to select one block of code from multiple options.

### Syntax

```java
switch(expression)
{
    case value:
        statements;
        break;

    default:
        statements;
}
```

### Example

```java
int day = 2;

switch(day)
{
    case 1:
        System.out.println("Monday");
        break;

    case 2:
        System.out.println("Tuesday");
        break;

    default:
        System.out.println("Invalid");
}
```

---

# 2. Iteration (Looping) Statements

Looping statements are used to execute a block of code repeatedly.

Types of Looping Statements

- while
- do-while
- for

---

## while Loop

The `while` loop executes as long as the condition is true.

### Syntax

```java
while(condition)
{
    // statements
}
```

### Example

```java
int i = 1;

while(i <= 5)
{
    System.out.println(i);
    i++;
}
```

---

## do-while Loop

The `do-while` loop executes the block at least once before checking the condition.

### Syntax

```java
do
{
    // statements
}
while(condition);
```

### Example

```java
int i = 1;

do
{
    System.out.println(i);
    i++;
}
while(i <= 5);
```

---

## for Loop

The `for` loop is used when the number of iterations is known.

### Syntax

```java
for(initialization; condition; increment/decrement)
{
    // statements
}
```

### Example

```java
for(int i = 1; i <= 5; i++)
{
    System.out.println(i);
}
```

---

# 3. Jump Statements

Jump statements are used to transfer the control of execution.

Types of Jump Statements

- break
- continue

---

## break Statement

The `break` statement is used to terminate the loop or switch statement immediately.

### Example

```java
for(int i = 1; i <= 5; i++)
{
    if(i == 3)
    {
        break;
    }

    System.out.println(i);
}
```

---

## continue Statement

The `continue` statement skips the current iteration and continues with the next iteration.

### Example

```java
for(int i = 1; i <= 5; i++)
{
    if(i == 3)
    {
        continue;
    }

    System.out.println(i);
}
```

---

# Quick Revision

- Control Statement → Controls the flow of execution.
- Selection → if, if-else, else-if, nested if, switch.
- Iteration → while, do-while, for.
- Jump → break, continue.

---
