# CS101 Spring 2026 — Practice Midterm Reflection

Name: Md. Nehal Uddin Rafin
Date: March 16, 2026

After completing the practice test, please reflect on your experience by
answering the questions below. Replace each `TODO` with a thoughtful response
(a few sentences each). Your responses help you consolidate what you learned
and identify areas to review before the real midterm.

---

## 1. Self-Assessment

**Question:** How did you feel about your performance on the practice test?
Which topics felt most comfortable, and which ones felt most difficult?

**Your Answer:**

Overall, I felt okay about my performance. Some questions felt straightforward, especially basic loops and simple conditions. I was more comfortable with things like lists and basic syntax. The harder parts for me were operator precedence and some of the data structure questions where I had to think more carefully.

---

## 2. Tricky Questions

**Question:** Identify one question you got wrong (or were unsure about).
Explain the concept being tested and describe why the correct answer is right.

**Your Answer:**

One question I found tricky was the exponentiation one with 2 ** 2 ** 3. At first, I thought it would go left to right, but Python actually evaluates it right to left. So it becomes 2 ** (2 ** 3) which is 2 ** 8 = 256. I got confused at first, but after understanding how precedence works, it made more sense.

---

## 3. Loops and Iteration

**Question:** In your own words, explain the difference between `range(a, b, step)`
with a positive step versus a negative step. Give one original example of each.

**Your Answer:**

The difference between a positive and negative step in range() is the direction the loop goes. With a positive step, the numbers increase, and with a negative step, they decrease.

Example with positive step:
for i in range(1, 6, 1):
    print(i)

Example with negative step:
for i in range(5, 0, -1):
    print(i)
---

## 4. Data Structures

**Question:** Python has lists, tuples, dictionaries, and sets. Describe one key
difference between a list and a tuple, and one key difference between a
dictionary and a set. When would you choose each?

**Your Answer:**

One key difference between a list and a tuple is that lists are mutable, but tuples are not. This means lists can be changed after creation, but tuples cannot. I would use a list when I need to modify data, and a tuple when I want the data to stay constant. One key difference between a list and a tuple is that lists are mutable, but tuples are not. This means lists can be changed after creation, but tuples cannot. I would use a list when I need to modify data, and a tuple when I want the data to stay constant.

---

## 5. Functions

**Question:** What is a default parameter in a Python function? Write a short
example function that uses a default parameter, and explain what happens when
the caller omits that argument.

**Your Answer:**

A default parameter is a value that a function uses if no argument is provided by the user.

Example:
def greet(name="Guest"):
    return "Hello " + name

If I call greet(), it will return "Hello Guest". If I call greet("Nehal"), it will return "Hello Nehal".
---

## 6. List Comprehensions

**Question:** List comprehensions can include an optional filter condition.
Rewrite the following traditional loop as a list comprehension:

```python
result = []
for n in range(1, 11):
    if n % 3 == 0:
        result.append(n * 2)
```

**Your Answer:**

result = [n * 2 for n in range(1, 11) if n % 3 == 0]

---

## 7. Operator Precedence

**Question:** Python evaluates `**` (exponentiation) right-to-left.
What is the value of `2 ** 2 ** 3`? Show your step-by-step reasoning.

**Your Answer:**

Python evaluates exponentiation from right to left.

So:
2 ** 2 ** 3

becomes:
2 ** (2 ** 3)

Then:
2 ** 8 = 256
---

## 8. Classes 

**Question:** What are classes in Python programming? Explain why they are necessary in programming.

**Your Answer:**

Classes are used to create objects that group data and functions together. They help organize code and make it easier to manage more complex programs. For example, instead of using separate variables, we can store everything related to something in one class. This makes the code cleaner and more reusable.

---

(Did you remember to add your name and date at the top of this document?)
Yes