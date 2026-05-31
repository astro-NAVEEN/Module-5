# Destructor in Python

This project demonstrates how to implement a **destructor** in Python using a simple class.

## 🚀 Overview

The program defines a class `Demo` with:

- A **constructor** `__init__` that initializes an instance variable and prints a message.
- A **destructor** `__del__` that prints a message when the object is destroyed.

## 🧠 Algorithm

1. Define a class named `Demo`.
2. Inside the class, define the `__init__` method:
   - Initialize an instance variable `status` with the value `"Alive"`.
   - Print the value of `status`.
3. Define the `__del__` method:
   - Print a message indicating the object is being destroyed.
4. Outside the class:
   - Create an instance of the `Demo` class.
   - Delete the object using the `del` keyword.
## Program

# Destructor in Python

class Demo:

    def __init__(self):
        self.status = "Alive"
        print(self.status)

    def __del__(self):
        print("Object is being destroyed")

obj = Demo()

del obj

## 🧪 Output
<img width="441" height="375" alt="Screenshot 2026-05-31 113352" src="https://github.com/user-attachments/assets/675decd2-80a7-473d-bf76-f658054f17f3" />


## Result
Thus, the Python program demonstrating the use of a constructor and destructor in a class was written and executed successfully.

