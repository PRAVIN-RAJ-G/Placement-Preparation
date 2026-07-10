
# ☕ Arrays in Java

## What is an Array?

An array is a collection of elements of the same data type stored in contiguous memory locations.

It is used to store multiple values using a single variable name.

---

# Why do we use Arrays?

Without arrays, we need to create separate variables to store multiple values.

### Without Array

```java
int mark1 = 85;
int mark2 = 90;
int mark3 = 95;
```

### With Array

```java
int[] marks = {85, 90, 95};
```

---

# Characteristics of Arrays

- Stores elements of the same data type.
- Array size is fixed.
- Elements are stored in contiguous memory.
- Index starts from **0**.

---

# Declaration of an Array

### Syntax

```java
dataType[] arrayName;
```

### Example

```java
int[] numbers;
```

---

# Array Creation

### Syntax

```java
arrayName = new dataType[size];
```

### Example

```java
numbers = new int[5];
```

---

# Array Initialization

```java
numbers[0] = 10;
numbers[1] = 20;
numbers[2] = 30;
numbers[3] = 40;
numbers[4] = 50;
```

---

# Declaration, Creation and Initialization in One Statement

```java
int[] numbers = {10, 20, 30, 40, 50};
```

---

# Accessing Array Elements

Array elements are accessed using their index.

### Example

```java
int[] numbers = {10, 20, 30};

System.out.println(numbers[0]);
System.out.println(numbers[1]);
System.out.println(numbers[2]);
```

---

# Traversing an Array

A loop is commonly used to access all elements of an array.

### Example

```java
int[] numbers = {10, 20, 30, 40, 50};

for(int i = 0; i < numbers.length; i++)
{
    System.out.println(numbers[i]);
}
```

---

# Advantages of Arrays

- Stores multiple values using one variable.
- Easy to access elements using an index.
- Reduces code repetition.
- Improves program readability.

---

# Limitations of Arrays

- Fixed size.
- Stores only one data type.
- Insertion and deletion are difficult.

---

# Quick Revision

- Array → Collection of same data type.
- Index starts from **0**.
- Size is fixed.
- Elements are stored in contiguous memory.
- Access elements using index.

---

# Interview Questions

1. What is an array?
2. Why do we use arrays?
3. What is array indexing?
4. Why does array indexing start from 0?
5. What are the advantages and limitations of arrays?
