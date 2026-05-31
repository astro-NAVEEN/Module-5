# Hierarchical Inheritance in Python

This Python project demonstrates **Hierarchical Inheritance** using a base class `Details` and two derived classes `Employee` and `Patient`. The program collects and displays details for both employees and patients.

## 🎯 Aim

To write a Python program that uses **Hierarchical Inheritance** to input and display **Employee** and **Patient** details.

## 📘 Description

- **Base Class:** `Details`
  - Stores common attributes: `name`, `age`
  - Provides methods: `getName()`, `getAge()`

- **Derived Class 1:** `Employee`
  - Inherits from `Details`
  - Adds: `employee_id`, `department`
  - Method: `getEmployeeDetails()`

- **Derived Class 2:** `Patient`
  - Inherits from `Details`
  - Adds: `patient_id`, `disease`
  - Method: `getPatientDetails()`

## 🧠 Algorithm

1. Create base class `Details` with common attributes.
2. Create `Employee` class extending `Details`, adding employee-specific data.
3. Create `Patient` class extending `Details`, adding patient-specific data.
4. Get user input for employee and patient data.
5. Display collected information using class methods.

## Program

# Hierarchical Inheritance in Python

class Details:
    def getName(self):
        self.name = input("Enter name: ")

    def getAge(self):
        self.age = int(input("Enter age: "))


class Employee(Details):
    def getEmployeeDetails(self):
        self.getName()
        self.getAge()
        self.employee_id = input("Enter employee ID: ")
        self.department = input("Enter department: ")

    def displayEmployee(self):
        print("\n--- Employee Details ---")
        print("Name:", self.name)
        print("Age:", self.age)
        print("Employee ID:", self.employee_id)
        print("Department:", self.department)


class Patient(Details):

    def getPatientDetails(self):
        self.getName()
        self.getAge()
        self.patient_id = input("Enter patient ID: ")
        self.disease = input("Enter disease: ")

    def displayPatient(self):
        print("\n--- Patient Details ---")
        print("Name:", self.name)
        print("Age:", self.age)
        print("Patient ID:", self.patient_id)
        print("Disease:", self.disease)


# Object creation and execution

e = Employee()

e.getEmployeeDetails()

e.displayEmployee()

p = Patient()

p.getPatientDetails()

p.displayPatient()

## Sample Output
<img width="660" height="508" alt="Screenshot 2026-05-31 143719" src="https://github.com/user-attachments/assets/f80afc1f-3da7-4aef-8f09-6dd7967ea78a" />

## RESULT 
Thus, the Python program demonstrating Hierarchical Inheritance using Details, Employee, and Patient classes was written and executed successfully.
