# Multilevel Inheritance Example in Python

This Python project demonstrates the concept of **Multilevel Inheritance** to collect and display the **name**, **age**, and **location** of a person.

## 🎯 Aim

To write a Python program that uses multilevel inheritance to get and display a person’s name, age, and location.

## 🧠 Algorithm

1. **Parent Class**  
   - `__init__(name)` initializes the `name` attribute.  
   - `getName()` returns the `name`.

2. **Child Class (inherits Parent)**  
   - `__init__(name, age)` initializes `name` using `super()` and adds `age`.  
   - `getAge()` returns the `age`.

3. **Grandchild Class (inherits Child)**  
   - `__init__(name, age, location)` initializes `name` and `age` using `super()` and adds `location`.  
   - `getLocation()` returns the `location`.

4. **Input & Output**  
   - Take user input for name, age, and location.  
   - Create an instance of `Grandchild`.  
   - Print all details using class methods.

## Program
# Multilevel Inheritance Example in Python

class Parent:

    def __init__(self, name):
        self.name = name

    def getName(self):
        return self.name


class Child(Parent):

    def __init__(self, name, age):
        super().__init__(name)
        self.age = age

    def getAge(self):
        return self.age


class Grandchild(Child):

    def __init__(self, name, age, location):
        super().__init__(name, age)
        self.location = location

    def getLocation(self):
        return self.location


# User input

name = input("Enter name: ")

age = int(input("Enter age: "))

location = input("Enter location: ")

# Object creation

person = Grandchild(name, age, location)

# Output
print("\n--- Person Details ---")

print("Name:", person.getName())

print("Age:", person.getAge())

print("Location:", person.getLocation())

## Sample Output
<img width="590" height="448" alt="Screenshot 2026-05-31 144102" src="https://github.com/user-attachments/assets/2ad788b1-de1e-4533-bcd0-a9997ee41855" />

## RESULT
Thus, the Python program demonstrating Multilevel Inheritance using name, age, and location was written and executed successfully.
