---
tags:
  - computer-science
  - advance
  - oop
  - ipst
source: "IPST (สสวท.) Computer Science Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว332"]
---

# Object-Oriented Programming — การเขียนโปรแกรมเชิงวัตถุ

> *"Object-oriented programming is an exceptionally bad idea which could only have originated in California."* — Edsger Dijkstra (famously critical, yet OOP dominates industry)

Object-Oriented Programming (การเขียนโปรแกรมเชิงวัตถุ, OOP) is a programming paradigm built around **objects** (วัตถุ) — bundles of related data (attributes) and behavior (methods). Instead of loose variables and functions scattered across a program, OOP groups them into coherent units that model real-world entities: a `Student`, a `BankAccount`, a `Car`. This makes large programs easier to organize, extend, and maintain.

Python is a multi-paradigm language with first-class OOP support. This note covers the four pillars — **encapsulation**, **inheritance**, **polymorphism**, and **abstraction** — using Python's class syntax, the `self` parameter, the `__init__` constructor, and practical patterns like composition vs inheritance.

---

## 1 | Course Coverage

### ม.5 (ว332)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Classes, objects, `__init__`, `self`, attributes and methods | Define a class, instantiate, call methods |
| **Semester 2** | Encapsulation, inheritance, polymorphism, composition | Override methods, use `super()`, design class hierarchies |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| คลาส | Class | Blueprint / template |
| ออบเจกต์ / วัตถุ | Object / Instance | Concrete thing made from a class |
| แอตทริบิวต์ | Attribute | Data stored in an object |
| เมธอด | Method | Function belonging to a class |
| ผู้สร้าง / คอนสตรักเตอร์ | Constructor | `__init__` — runs at creation |
| การห่อหุ้ม | Encapsulation | Hide internal data |
| การสืบทอด | Inheritance | Child reuses parent code |
| ความหลากสภาพ | Polymorphism | Same interface, different behavior |
| การทำสิ่งเชิงนามธรรม | Abstraction | Expose essentials, hide details |
| คลาสแม่ / คลาสลูก | Parent / Child class | superclass / subclass |
| การประกอบ | Composition | "Has-a" relationship |

---

## 3 | Key Concepts

### 3.1 Classes and Objects (คลาสและออบเจกต์)

A **class** (คลาส) is a blueprint; an **object** (ออบเจกต์) is a concrete instance built from that blueprint.

```python
class Dog:
    def __init__(self, name, age):   # constructor
        self.name = name             # attribute
        self.age = age

    def bark(self):                  # method
        return f"{self.name} says Woof!"

d1 = Dog("Bingo", 3)     # create object (instance)
d2 = Dog("Lucky", 5)
print(d1.bark())         # "Bingo says Woof!"
print(d2.age)            # 5
```

### 3.2 The `__init__` Constructor and `self`

- `__init__` (คอนสตรักเตอร์) is the **special method** Python calls automatically when you create an object. It initializes attributes.
- `self` (ตัวมันเอง) refers to **the current object** — the specific instance the method is acting on. It must be the first parameter of every instance method, though Python passes it automatically.

```python
class Student:
    def __init__(self, name, score):
        self.name = name
        self.score = score

    def grade(self):
        return "Pass" if self.score >= 50 else "Fail"

s = Student("Somchai", 78)
print(s.grade())   # "Pass"
```

### 3.3 Attributes and Methods

- **Instance attributes** (แอตทริบิวต์ของอินสแตนซ์) — unique per object, set in `__init__` via `self.x = ...`.
- **Class attributes** (แอตทริบิวต์ของคลาส) — shared by all instances, defined directly in the class body.

```python
class Counter:
    total = 0               # class attribute (shared)
    def __init__(self):
        self.count = 0      # instance attribute (per object)
        Counter.total += 1
```

### 3.4 Encapsulation (การห่อหุ้ม)

Encapsulation (การห่อหุ้ม) hides internal state and exposes only controlled access. Python uses a **naming convention**: a leading underscore `_x` signals "private by agreement"; a double underscore `__x` triggers **name mangling** (เนมแมงกลิง) for stronger protection.

```python
class BankAccount:
    def __init__(self, owner, balance):
        self.owner = owner
        self.__balance = balance      # name-mangled, "private"

    def deposit(self, amount):
        if amount > 0:
            self.__balance += amount

    def get_balance(self):
        return self.__balance

acct = BankAccount("Anna", 1000)
acct.deposit(500)
print(acct.get_balance())   # 1500
# acct.__balance            # AttributeError — protected
```

### 3.5 Inheritance (การสืบทอด)

Inheritance (การสืบทอด) lets a **child class** (คลาสลูก) reuse and extend a **parent class** (คลาสแม่). Use `super()` to call the parent's constructor or methods.

```python
class Animal:
    def __init__(self, name):
        self.name = name
    def speak(self):
        return "..."

class Cat(Animal):                 # Cat inherits from Animal
    def speak(self):               # override
        return f"{self.name} says Meow"

class Dog(Animal):
    def speak(self):
        return f"{self.name} says Woof"

c = Cat("Kitty")
print(c.speak())   # "Kitty says Meow"
```

### 3.6 Polymorphism (ความหลากสภาพ)

Polymorphism (ความหลากสภาพ) means "many forms": different classes can share the same method name yet behave differently. The caller does not need to know the exact type.

```python
def make_speak(animal):
    print(animal.speak())          # works for Cat, Dog, any Animal

for a in [Cat("Kitty"), Dog("Bingo")]:
    make_speak(a)
# Kitty says Meow
# Bingo says Woof
```

### 3.7 Composition vs Inheritance

- **Inheritance** models an **"is-a"** relationship: a `Cat` *is an* `Animal`.
- **Composition** (การประกอบ) models a **"has-a"** relationship: a `Car` *has an* `Engine`. Prefer composition when classes do not share a true subtype relationship.

```python
class Engine:
    def start(self):
        return "Engine running"

class Car:
    def __init__(self):
        self.engine = Engine()    # composition: Car HAS-A Engine
    def start(self):
        return self.engine.start() + " — Car ready"

print(Car().start())   # "Engine running — Car ready"
```

---

## 4 | Common Problem Types

### Type 1: Design a Bank Account Class

> Create a `BankAccount` with deposit, withdraw (reject overdraft), and balance display.

**Solution:**
```python
class BankAccount:
    def __init__(self, owner, balance=0):
        self.owner = owner
        self.__balance = balance

    def deposit(self, amount):
        if amount > 0:
            self.__balance += amount

    def withdraw(self, amount):
        if 0 < amount <= self.__balance:
            self.__balance -= amount
        else:
            print("Insufficient funds or invalid amount")

    def show(self):
        return f"{self.owner}: {self.__balance} THB"

acct = BankAccount("Nicha", 500)
acct.deposit(200)
acct.withdraw(1000)   # rejected
print(acct.show())    # Nicha: 700 THB
```

### Type 2: Shape Hierarchy with Polymorphism

> Define `Shape` with subclasses `Circle` and `Rectangle`, each computing its own `area()`.

**Solution:**
```python
import math

class Shape:
    def area(self):
        raise NotImplementedError

class Circle(Shape):
    def __init__(self, r):
        self.r = r
    def area(self):
        return math.pi * self.r ** 2

class Rectangle(Shape):
    def __init__(self, w, h):
        self.w = w
        self.h = h
    def area(self):
        return self.w * self.h

shapes = [Circle(3), Rectangle(4, 5)]
for s in shapes:
    print(f"Area = {s.area():.2f}")
# Area = 28.27
# Area = 20.00
```

### Type 3: Student Grade System with Inheritance

> A base `Person` has a name; `Student` extends it with scores and a grade computation.

**Solution:**
```python
class Person:
    def __init__(self, name):
        self.name = name

class Student(Person):
    def __init__(self, name, score):
        super().__init__(name)      # call parent constructor
        self.score = score

    def grade(self):
        if self.score >= 80:  return "A"
        if self.score >= 70:  return "B"
        if self.score >= 60:  return "C"
        if self.score >= 50:  return "D"
        return "F"

s = Student("Ploy", 85)
print(f"{s.name}: {s.grade()}")   # Ploy: A
```

---

## 5 | Cross-Links

- [[07_Data_Structures]] — implement structures (Stack, Node) as classes
- [[06_Algorithms]] — OOP organizes algorithm logic into methods
- [[10_Databases]] — ORM models map tables to objects
- [[11_Artificial_Intelligence]] — ML models are OOP objects (`.fit()`, `.predict()`)
