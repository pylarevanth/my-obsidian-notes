
---
# 1. Operators

Operators are symbols/keywords used to perform operations on values.

Python operators can be grouped into:

```
Arithmetic
Comparison
Logical
Assignment
Bitwise
Membership
Identity
```

---

## 1.1 Arithmetic Operators

Used for mathematical operations.

```
a = 10
b = 3

a + b    # 13
a - b    # 7
a * b    # 30
a / b    # 3.333...
a // b   # 3
a % b    # 1
a ** b   # 1000
```

### Important: `/` vs `//`

```
10 / 3     # 3.333...
10 // 3    # 3
```

`/` performs **true division**.

`//` performs **floor division**.

---

## 1.2 Comparison Operators

Used to compare values.

```
a = 10
b = 20

a == b    # False
a != b    # True
a > b     # False
a < b     # True
a >= b    # False
a <= b    # True
```

Comparison operators return a Boolean:

```
True
False
```

---

## 1.3 Logical Operators

Used to combine conditions.

### `and`

Returns true when **both** conditions are true.

```
age = 22
has_id = True

age >= 18 and has_id
# True
```

### `or`

Returns true when **at least one** condition is true.

```
age >= 18 or has_id
```

### `not`

Reverses the Boolean result.

```
not True
# False
```

---

# 2. Short-Circuit Evaluation

This is an important interview concept.

Python doesn't necessarily evaluate every condition.

```
False and some_function()
```

Since the first condition is already `False`, Python knows the entire expression must be false.

So `some_function()` isn't executed.

Similarly:

```
True or some_function()
```

doesn't need to evaluate `some_function()`.

This is called **short-circuit evaluation**.

---

# 3. Assignment Operators

Basic:

```
x = 10
```

Compound assignment:

```
x += 5
x -= 2
x *= 3
x /= 2
x //= 2
x %= 2
x **= 2
```

For example:

```
x = 10
x += 5

print(x)
```

Output:

```
15
```

---

# 4. Membership Operators

Used to check whether a value exists inside a collection.

```
numbers = [1, 2, 3, 4]

2 in numbers
# True

10 in numbers
# False
```

`not in` checks the opposite.

```
10 not in numbers
# True
```

You'll use this frequently with:

- lists
- sets
- dictionaries
- strings

---

# 5. Identity Operators

Python has:

```
is
is not
```

They check **object identity**, not value equality.

```
a = [1, 2]
b = [1, 2]

a == b    # True
a is b    # False
```

Why?

The two lists contain equal values but are different objects.

We'll cover `is` vs `==` in much greater depth later because it's an important interview topic.

---

# 6. Input and Output

## `input()`

Used to receive user input.

```
name = input("Enter your name: ")
```

### Important interview point

`input()` **always returns a string**.

```
age = input("Enter age: ")

print(type(age))
```

Output:

```
<class 'str'>
```

If you need an integer:

```
age = int(input("Enter age: "))
```

---

# 7. Output with `print()`

```
name = "Alex"
age = 21

print(name)
print(age)
```

Multiple values:

```
print(name, age)
```

---

## f-strings

The preferred way to construct formatted strings in modern Python:

```
name = "Alex"
age = 21

print(f"My name is {name} and I am {age} years old.")
```

Output:

```
My name is Alex and I am 21 years old.
```

---

# 8. Conditional Statements

Conditional statements allow your program to make decisions.

Basic structure:

```
if condition:
    # code
elif another_condition:
    # code
else:
    # code
```

Example:

```
age = 20

if age >= 18:
    print("Adult")
else:
    print("Minor")
```

---

# 9. Multiple Conditions

```
marks = 85

if marks >= 90:
    grade = "A"
elif marks >= 75:
    grade = "B"
elif marks >= 60:
    grade = "C"
else:
    grade = "D"
```

Python evaluates conditions **from top to bottom** and executes the first matching branch.

---

# 10. Truthy and Falsy Values

Python allows objects to be evaluated directly in conditions.

Common falsy values:

```
False
None
0
0.0
""
[]
()
{}
set()
```

Most other objects are truthy.

Example:

```
name = ""

if name:
    print("Name exists")
else:
    print("Name is empty")
```

Output:

```
Name is empty
```

This is very common in real Python code.

---

# 📒 Revision Notes

### Operators

- Arithmetic → `+ - * / // % **`
- Comparison → `== != > < >= <=`
- Logical → `and or not`
- Assignment → `= += -= *= /= ...`
- Membership → `in`, `not in`
- Identity → `is`, `is not`

### Important distinctions

```
/   → true division
//  → floor division

==  → value equality
is  → object identity

in  → membership
```

### Input

```
input()
```

always returns a **string**.

### Conditions

```
if
elif
else
```

Python evaluates branches from top to bottom.

### Truthiness

Empty collections, `0`, `False`, and `None` are generally falsy.

---

# 🎤 Interview Vault

## Q1. What is the difference between `/` and `//`?

**Answer:**

`/` performs true division and returns a floating-point result, while `//` performs floor division and returns the floor of the division result.

```
10 / 3     # 3.333...
10 // 3    # 3
```

---

## Q2. What is the difference between `==` and `is`?

**Answer:**

`==` checks whether two objects have equal values, while `is` checks whether they refer to the same object in memory.

```
a = [1, 2]
b = [1, 2]

a == b    # True
a is b    # False
```

---

## Q3. What does `input()` return?

**Answer:**

`input()` always returns a string, even when the user enters a number.

```
age = input()
```

If an integer is required:

```
age = int(input())
```

---

## Q4. What is short-circuit evaluation?

**Answer:**

Short-circuit evaluation means Python stops evaluating a logical expression as soon as its result is known.

For example:

```
False and expensive_operation()
```

The second expression isn't evaluated because the result must already be `False`.

---

## Q5. What are truthy and falsy values?

**Answer:**

Python objects can be evaluated as Boolean values. Values such as `False`, `None`, `0`, empty strings, and empty collections are falsy, while most other values are truthy.

---

## Q6. How does Python evaluate an `if-elif-else` chain?

**Answer:**

Python evaluates the conditions from top to bottom and executes the first condition that evaluates to true. Once a branch executes, the remaining branches are skipped.

---

## Q7. What is the difference between `and` and `or`?

**Answer:**

`and` requires both operands to satisfy the condition, while `or` requires at least one. Python also short-circuits these expressions.

---

# 🔄 Interview Follow-ups

### Q: Why is this useful?

```
if data:
```

Instead of:

```
if len(data) > 0:
```

**Answer:**

Python's truth-value testing allows collections to be directly evaluated. An empty collection is falsy and a non-empty collection is truthy, making the first version concise and idiomatic.

---

### Q: Is `is` only used with objects?

**Answer:**

`is` checks object identity, so conceptually it is comparing whether two references point to the same object. It is commonly appropriate for singleton objects such as `None`.

```
if value is None:
    ...
```

---

### Q: Does `and` always return `True` or `False`?

**Answer:**

No. Python's `and` and `or` operators can return one of their operands.

```
x = 10 and 20
print(x)
```

Output:

```
20
```

This becomes particularly important when writing concise Python expressions.

---

# ⚠️ Common Interview Traps

### Trap 1

❌ "`==` checks memory address."

✅ `==` checks equality; `is` checks identity.

---

### Trap 2

❌ "`input()` automatically converts numbers."

✅ `input()` always returns `str`.

---

### Trap 3

❌ "`and` and `or` always return Boolean values."

✅ They can return one of their operands.

---

### Trap 4

❌ "`//` simply removes the decimal part."

Not always.

```
-7 // 2
```

Result:

```
-4
```

Because floor division rounds **toward negative infinity**, not toward zero.

---

# 💻 Coding Practice

### Problem 1 — Grade Calculator

Write a program that takes marks and prints:

```
90+  → A
75-89 → B
60-74 → C
40-59 → D
<40  → F
```

---

### Problem 2 — Number Checker

Given a number, determine whether it is:

- positive
- negative
- zero
- even or odd

---

### Problem 3 — Data Science Style

Given:

```
age = 25
experience = 2
```

Write a condition that returns `"Eligible"` if:

- age >= 18
- experience >= 1

Otherwise return `"Not Eligible"`.

---

# 🔗 Data Science Connection

Conditions appear throughout ML/data pipelines:

```
if df.empty:
    ...
```

```
if missing_percentage > 50:
    ...
```

```
if accuracy >= threshold:
    ...
```

And operators become especially important when filtering Pandas DataFrames:

```
df[df["age"] > 25]
```

Later we'll connect Python logical operators with **Pandas boolean masking**, where there are some important differences such as using `&` and `|` instead of Python's `and` and `or`.

---

# 🧠 Recall Checklist

You should now know:

- Arithmetic operators
- Comparison operators
- Logical operators
- Assignment operators
- Membership operators
- Identity operators
- `/` vs `//`
- `==` vs `is`
- `input()`
- f-strings
- `if / elif / else`
- Truthy/falsy values
- Short-circuit evaluation
- `and` / `or` operand behavior

---
### ✅ Phase 0 Progress

**0.1 Python Core Revision**

- ✅ 0.1.1 Variables, Data Types & Type Conversion
- ✅ 0.1.2 Operators, Input/Output & Conditionals
- ⏭️ **Next: 0.1.3 Loops + `break` + `continue` + `pass`**

---
