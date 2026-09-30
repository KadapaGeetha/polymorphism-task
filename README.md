# polymorphism-task
# Python Polymorphism Tasks

## 📌 Project Overview

This repository contains a collection of **20 Python Object-Oriented Programming (OOP) tasks** focused mainly on **Polymorphism**.

The tasks cover:

* Method Overriding
* Polymorphism
* Duck Typing
* Built-in Polymorphism
* Class Methods
* Operator Overloading
* Custom Data Types
* Inheritance
* Common Functions
* List and Loop based polymorphism

All tasks are implemented in Python in the `polymorphism.py` file.

## 🛠️ Technologies Used

* Python
* Object-Oriented Programming (OOP)

## 📂 Project Structure

```text
polymorphism-task/
│
├── polymorphism.py
└── README.md
```

## 📚 Tasks Covered

### Q1. Animal Sound – Method Overriding

Created a parent class `Animal` and child classes:

* `Dog`
* `Cat`
* `Cow`

Each child class overrides the `sound()` method with its own implementation.

**Concept:** Method Overriding and Polymorphism

---

### Q2. Payment Processing

Created a parent class `Payment` and child classes:

* `UPI`
* `CreditCard`
* `Cash`

Each class implements its own `pay()` method.

**Concept:** Method Overriding and Polymorphism

---

### Q3. Employee Salary

Created a parent class `Employee` with child classes:

* `FullTimeEmployee`
* `PartTimeEmployee`

Each class calculates salary differently.

**Concept:** Method Overriding and Polymorphism

---

### Q4. Shape Area

Created a parent class `Shape` and child classes:

* `Circle`
* `Rectangle`
* `Square`

Each class calculates its area using its own implementation of `area()`.

**Concept:** Method Overriding

---

### Q5. Vehicle Start

Created a parent class `Vehicle` and child classes:

* `Car`
* `Bike`
* `Bus`

Each vehicle has a different implementation of `start()`.

A common function is used to call the method.

**Concept:** Polymorphism

---

### Q6. Calculator – Method with Different Arguments

Created a `Calculator` class with an `add()` method that accepts either two or three numbers using a default argument.

```python
def add(self, a, b, c=0):
```

**Concept:** Method Overloading using Default Arguments

---

### Q7. Notification System – Duck Typing

Created three unrelated classes:

* `EmailNotification`
* `SMSNotification`
* `WhatsappNotification`

Each class has a `send()` method.

A common `notify_user()` function calls `send()` without checking the object type.

**Concept:** Duck Typing

---

### Q8. Bank Interest Rate

Created a parent class `Bank` and child classes:

* `SBI`
* `HDFC`
* `ICICI`

Each bank provides a different `interest_rate()` implementation.

**Concept:** Method Overriding and Polymorphism

---

### Q9. Built-in Polymorphism

Created:

* List
* Tuple
* String
* Dictionary

Used the same built-in functions:

```python
len()
type()
```

on different object types.

**Concept:** Built-in Polymorphism

---

### Q10. Food Preparation

Created a parent class `Food` and child classes:

* `Pizza`
* `Burger`
* `Biryani`

Each class provides its own implementation of `prepare()`.

A common function calls the method for different food objects.

**Concept:** Polymorphism and Method Overriding

---

### Q11. Book Pages – Operator Overloading

Created a `Book` class with a `pages` attribute.

Overloaded the `+` operator using:

```python
__add__()
```

This allows two book objects to be added together to calculate their total pages.

Example:

```text
150 + 200 = 350 pages
```

**Concept:** Operator Overloading

---

### Q12. Product Price Comparison

Created a `Product` class with a `price` attribute.

Overloaded the `>` operator using:

```python
__gt__()
```

This allows two product objects to be compared based on price.

**Concept:** Operator Overloading

---

### Q13. Media Player – Duck Typing

Created three unrelated classes:

* `Audio`
* `Video`
* `Podcast`

Each class contains a `play()` method.

A common function accepts any object and calls its `play()` method without checking its class.

**Concept:** Duck Typing

---

### Q14. Employee Company Information – Class Method

Created a parent class `Employee` with a class method:

```python
company_info()
```

Created child classes:

* `Developer`
* `DataAnalyst`

Both child classes override the class method.

The method is called directly using the class name.

**Concept:** Class Method and Method Overriding

---

### Q15. Product Discount

Created three classes:

* `Electronics`
* `Clothing`
* `Grocery`

Each class has a `calculate_discount()` method with its own discount calculation.

A common function calculates and displays the final price.

**Concept:** Polymorphism

---

### Q16. Ride Fare Calculation

Created a parent class `Ride` and child classes:

* `BikeRide`
* `CarRide`
* `AutoRide`

Each ride calculates fare based on distance and its own rate per kilometer.

A common function displays the fare.

**Concept:** Method Overriding and Polymorphism

---

### Q17. Doctor Treatment

Created a parent class `Doctor` and child classes:

* `Cardiologist`
* `Dentist`
* `Neurologist`

Each doctor provides a different implementation of:

```python
treat_patient()
```

The objects are stored in a list and processed using a loop.

**Concept:** Polymorphism

---

### Q18. File Processing – Duck Typing

Created three classes:

* `CSVFile`
* `JSONFile`
* `TextFile`

Each class contains:

```python
read_file()
```

A common `process_file()` function accepts different file objects and calls the appropriate method.

**Concept:** Duck Typing

---

### Q19. Custom Data Type – Distance

Created a `Distance` class with:

```python
km
meters
```

Overloaded the `+` operator using:

```python
__add__()
```

Two distance objects are added and the result is normalized.

Example:

```text
Distance 1: 2 km 500 meters
Distance 2: 3 km 800 meters

Total: 6 km 300 meters
```

Since 1000 meters equals 1 kilometer, the extra kilometer is carried over automatically.

**Concept:** Operator Overloading and Custom Data Types

---

### Q20. Complete Polymorphism Challenge

Created a parent class `Employee` and child classes:

* `Manager`
* `Developer`
* `Tester`

Each employee provides its own implementation of:

```python
work()
calculate_bonus()
display_details()
```

All employee objects are stored in a list and processed using a loop without checking their object type.

**Concept:** Inheritance, Method Overriding, and Polymorphism

## 🧠 Key Concepts Learned

### 1. Method Overriding

A child class provides its own implementation of a method already defined in the parent class.

Example:

```python
class Animal:
    def sound(self):
        print("Animal sound")


class Dog(Animal):
    def sound(self):
        print("Bow Bow")
```

### 2. Polymorphism

The same method name can perform different actions depending on the object.

```python
for employee in employees:
    employee.work()
```

The correct `work()` method is automatically called for each object.

### 3. Duck Typing

Python focuses on whether an object has the required method rather than checking its class.

```python
def process_file(file):
    file.read_file()
```

Any object with `read_file()` can be passed to the function.

### 4. Operator Overloading

Python operators can be customized for user-defined objects.

Examples:

```python
__add__()
__gt__()
```

This allows expressions such as:

```python
book1 + book2
```

and:

```python
product1 > product2
```

### 5. Class Methods

Class methods use the `@classmethod` decorator and work with the class rather than a particular object.

```python
@classmethod
def company_info(cls):
    print("Company Information")
```

## ▶️ How to Run

Make sure Python is installed on your system.

Run the following command from the project folder:

```bash
python polymorphism.py
```

The program will execute the different polymorphism exercises and display their outputs.

## 🎯 Learning Outcome

After completing these tasks, I practiced how Python handles different objects through a common interface.

The exercises helped me understand:

* How inheritance works
* How method overriding works
* How polymorphism allows the same method call to behave differently
* How duck typing works without inheritance
* How built-in functions work with different data types
* How operators can be overloaded
* How class methods work
* How common functions can work with different objects

## 👩‍💻 Author

**Geetha Kadapa**

Python | OOP | Polymorphism Practice
