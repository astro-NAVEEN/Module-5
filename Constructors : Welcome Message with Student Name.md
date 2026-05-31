# # Constructors in Python: Welcome Message with Student Name

## 🎯 Aim
To write a Python program that creates a **Student** class with a **default constructor** and a method to display a welcome message along with the student’s name provided by the user.

## 🧠 Algorithm
1. **Get user input**: Accept the student's name from the user.
2. **Define the class**: Create a class `Student` with a default constructor (`__init__`).
3. **Default Constructor**: In the constructor, assign the user input (student name) to an instance variable `self.a`.
4. **Display Message**: Define a method `show` that prints "This is non-parameterized constructor" and a welcome message with the student’s name.
5. **Execute the Program**: Instantiate the `Student` class and call the `show` method.

## 🧾 Program

# Constructors in Python: Welcome Message with Student Name

class Student:

    def __init__(self, name):
        self.a = name

    def show(self):
        print("This is non-parameterized constructor")
        print("Welcome", self.a)

name = input("Enter student name: ")

s1 = Student(name)
s1.show()

## Output
<img width="623" height="366" alt="Screenshot 2026-05-31 113207" src="https://github.com/user-attachments/assets/27887f06-63a4-4786-bf5d-7d795bc3fa0f" />


## Result
Thus, the Python program using a class with a constructor to display a welcome message along with the student’s name was written and executed successfully.
