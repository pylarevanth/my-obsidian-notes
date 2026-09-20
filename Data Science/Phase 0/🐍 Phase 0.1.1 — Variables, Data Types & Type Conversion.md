
---
# 1. Variables

### Concept

A variable in Python is a **name/reference bound to an object**.

```
x = 10
```

Here:

- `10` is an object
- `x` is the name referring to that object
- Python determines the type at runtime

### Important mental model

```
x ───────► 10
           object
```

Python variables don't have a fixed type themselves. The **object has a type**.

```
x = 10
x = "hello"
```

The name `x` is first bound to an integer object and later rebound to a string object.

---

# 2. Python Data Types

### Main built-in types

|Category|Types|
|---|---|
|Numeric|`int`, `float`, `complex`|
|Boolean|`bool`|
|Text|`str`|
|Sequence|`list`, `tuple`, `range`|
|Set|`set`, `frozenset`|
|Mapping|`dict`|
|Binary|`bytes`, `bytearray`|
|Special|`NoneType`|

Examples:

```
age = 21                    # int
price = 99.5                # float
z = 2 + 3j                  # complex
is_active = True            # bool
name = "Revan"              # str

numbers = [1, 2, 3]         # list
point = (10, 20)            # tuple
unique = {1, 2, 3}          # set

student = {"name": "Alex"}  # dict

result = None               # NoneType
```

---

# 3. Dynamic Typing

Python is **dynamically typed**.

The type of an object is determined during runtime.

```
x = 10
x = "Python"
x = [1, 2, 3]
```

The name `x` can refer to objects of different types.

Check the type:

```
type(x)
```

---

# 4. Strong Typing

Python is also **strongly typed**.

It doesn't automatically perform unrelated type conversions.

```
x = "10"
y = 5

x + y
```

This produces:

```
TypeError
```

You must explicitly convert:

```
int(x) + y
```

Result:

```
15
```

---

# 5. Type Conversion

Type conversion means converting one data type into another.

### Common conversions

```
int("10")        # 10
float("10.5")    # 10.5
str(100)         # "100"
bool(1)          # True
list("abc")      # ['a', 'b', 'c']
tuple([1, 2])    # (1, 2)
set([1, 2, 2])   # {1, 2}
```

### Important distinction

**Implicit conversion**

Python automatically converts in certain compatible numeric operations:

```
x = 10
y = 2.5

x + y
```

Result:

```
12.5
```

`int` is promoted to `float`.

**Explicit conversion**

You manually convert:

```
x = "10"
x = int(x)
```

---

# 📒 Revision Notes

### Variables

- Variable = name bound to an object.
- Python variables don't have fixed types.
- Objects have types.
- Assignment creates/rebinds references.

### Python Typing

- Python → dynamically typed
- Python → strongly typed
- Type determined at runtime.
- Different types can be assigned to the same variable name.

### Type Conversion

- `int()`
- `float()`
- `str()`
- `bool()`
- `list()`
- `tuple()`
- `set()`

---

# 🎤 Interview Vault

## Q1. Is Python statically typed or dynamically typed?

**Answer:**

Python is dynamically typed because variable types are determined at runtime, and the same variable name can refer to objects of different types during execution.

```
x = 10
x = "hello"
```

---

## Q2. Is Python strongly typed or weakly typed?

**Answer:**

Python is strongly typed because it does not automatically combine incompatible types.

```
"10" + 5
```

raises a `TypeError` instead of automatically converting the integer to a string.

---

## Q3. What is a variable in Python?

**Answer:**

A Python variable is a name that refers to an object in memory. The variable itself doesn't have a fixed type; the object it refers to has a type.

---

## Q4. What happens when you execute `x = 10`?

**Answer:**

Python creates or uses an integer object representing `10` and binds the name `x` to that object. If `x` was previously referring to another object, the name is rebound to the new object.

---

## Q5. Can a Python variable change its type?

**Answer:**

Yes. Python is dynamically typed, so a variable name can refer to objects of different types at different times.

```
x = 10
x = "hello"
```

---

## Q6. What is the difference between dynamic typing and strong typing?

**Answer:**

Dynamic typing means type checking happens at runtime and variables don't have fixed types. Strong typing means Python doesn't freely perform incompatible type conversions.

---

## Q7. What is type conversion?

**Answer:**

Type conversion is the process of converting a value from one data type to another, either explicitly using functions like `int()`, `float()`, and `str()`, or implicitly when Python performs certain compatible numeric conversions.

---

## Q8. What is the difference between implicit and explicit type conversion?

**Answer:**

Implicit conversion is performed automatically by Python when appropriate, while explicit conversion is performed manually by the programmer.

```
# Implicit
10 + 2.5

# Explicit
int("10")
```

---

# 🔄 Interview Follow-ups

### Follow-up 1

**Why doesn't `"10" + 5` work?**

Because Python doesn't automatically convert unrelated types in this situation. They are incompatible operands for string concatenation.

---

### Follow-up 2

**Does dynamic typing mean Python doesn't perform type checking?**

No.

Python performs type checking at runtime.

For example:

```
"10" + 5
```

results in a runtime `TypeError`.

---

### Follow-up 3

**Is everything in Python an object?**

Almost everything you work with in Python is an object, including numbers, strings, functions, classes, lists, and modules.

---

# ⚠️ Common Interview Traps

### ❌ Wrong

> "Python variables have a data type."

### ✅ Better

> Python variables are names bound to objects, and the objects have types.

---

### ❌ Wrong

> "Python is weakly typed because it is dynamically typed."

### ✅ Correct

> Dynamic typing and weak/strong typing are different concepts. Python is dynamically typed and strongly typed.

---

### ❌ Wrong

> "Python converts any incompatible types automatically."

### ✅ Correct

> Python performs some implicit numeric conversions, but it does not automatically convert arbitrary incompatible types.

---

# 💻 Coding Practice

### Problem 1

Write Python code that:

1. Creates an integer
2. Converts it to a float
3. Converts it to a string
4. Converts the string back to an integer
5. Prints the type after every conversion

### Problem 2

Predict the output:

```
x = 10
x = "20"

print(x)
print(type(x))
```

### Problem 3

What happens here?

```
x = "100"
y = 20

print(x + y)
```

Explain why.

---

# 🔗 Data Science Connection

These fundamentals appear everywhere in Data Science.

For example, when loading a dataset:

```
df["age"]
```

the values have a particular dtype.

Incorrect data types can affect:

- Pandas operations
- numerical calculations
- missing-value handling
- model training
- memory usage
- preprocessing pipelines

So understanding Python's type system becomes important when we later move into **NumPy → Pandas → ML preprocessing**.

---

# 🧠 Recall Checklist

Before moving forward, you should be able to explain:

- What is a Python variable?
- What is an object?
- What does `x = 10` actually mean?
- What does dynamically typed mean?
- What does strongly typed mean?
- Dynamic vs static typing
- Strong vs weak typing
- Explicit vs implicit conversion
- Common Python built-in data types
- Why `"10" + 5` raises an error

---
## ✅ 0.1 Progress

**Completed:** `0.1.1 Variables, Data Types & Type Conversion`

**Next:** `0.1.2 Operators + Input/Output + Conditional Statements`

---
