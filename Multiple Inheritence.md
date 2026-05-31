# Arithmetic Operations Using Multiple Inheritance in Python

This Python program demonstrates **multiple inheritance** by performing basic arithmetic operations — Addition, Subtraction, and Division — using three classes.

## 🎯 Aim

To write a Python program to calculate **Add, Sub & Division** using **Multiple Inheritance**.

## 🧠 Algorithm

1. **Define `Calculation1` class**
   - Contains `Summation(a, b)` method to return the sum of two numbers.
2. **Define `Calculation2` class**
   - Contains `Subtraction(a, b)` method to return the difference of two numbers.
3. **Define `Derived` class**
   - Inherits from both `Calculation1` and `Calculation2`.
   - Contains `Division(a, b)` method to return the division result.
4. **Input**
   - Prompt the user to enter two numbers.
5. **Process**
   - Create an object of the `Derived` class.
   - Call `Summation`, `Subtraction`, and `Division` methods.
6. **Output**
   - Display the results of the three operations.

## 💻 Program 

# Arithmetic Operations Using Multiple Inheritance in Python

class Calculation1:

    def Summation(self, a, b):
        return a + b


class Calculation2:

    def Subtraction(self, a, b):
        return a - b


class Derived(Calculation1, Calculation2):

    def Division(self, a, b):
        if b != 0:
            return a / b
        else:
            return "Division by zero not allowed"


# Input
a = float(input("Enter first number: "))

b = float(input("Enter second number: "))

# Object creation
obj = Derived()

# Output
print("Addition:", obj.Summation(a, b))

print("Subtraction:", obj.Subtraction(a, b))

print("Division:", obj.Division(a, b))

## Output Example
<img width="673" height="429" alt="Screenshot 2026-05-31 144425" src="https://github.com/user-attachments/assets/32bc7788-6bd5-4efe-985a-6d75d6518f39" />

## RESULT
Thus, the Python program demonstrating Multiple Inheritance for arithmetic operations (addition, subtraction, and division) was written and executed successfully.
