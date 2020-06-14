
# Python Online Bootcamp

Till this moment we have experienced three sessions of the class and one session of TA.

List of class sessions:
- [Session 2](#session-2)
    - [2.1 Object Class](#21-object-class), [2.2 Type Meta-Class](#22-type-meta-class), [2.3 Overloading vs. Overriding](#23-overloading-vs-overriding), [2.4 Inheritance vs. Instantiation from Meta-Class](#24-inheritance-vs-instantiation-from-meta-class), [2.5 Gang of Three Methods](#25-gang-of-three-methods), [2.6 When to Define Meta-Class](#26-when-to-define-meta-class), [2.7 Gang of Three Method Types!](#27-gang-of-three-method-types), [2.8 Design Patterns](#28-design-patterns), [2.9 Singleton Design Pattern](#29-singleton-design-pattern)
- [TA 1](#ta-1)
    - [TA1.1 Method Resolution Order](#ta11-method-resolution-order), [TA1.2 Factory Design Pattern](#ta12-factory-design-pattern), [TA1.3 Abstract Classes (_abc_ Module)](#ta13-abstract-classes-_abc_-module)
- [Session 3](#session-3)

    - [3.1 Observer Design Pattern](#31-observer-design-pattern), [3.2 UML](#32-uml), [3.3 BFS Algorithm for Graph Class of Previous Session](#33-bfs-algorithm-for-graph-class-of-previous-session), [3.4 Coupling (and IOC) vs Cohesion](#34-coupling-and-ioc-vs-cohesion), [3.5 Abstract Class](#35-abstract-class), [3.6 Closure in Python](#36-closure-in-python), [3.7 Linter in Text Editors](#37-linter-in-text-editors), [3.8 Abstract Classes Vs. Interfaces](#38-abstract-classes-vs-interfaces), [3.9 Decorators](#39-decorators), [3.10 Decorators with Arguments](#310-decorators-with-arguments)

---

## Session 2

----

### 2.1 Object Class
**issubclass** and **isinstance** functions
```python
int_instance = 13
str_instance = 'hi!'

print(issubclass(int, object)) # True
print(issubclass(int_instance, object)) # Error
print(issubclass(int, int)) # True
print(issubclass(int_instance, int)) # Error
print(isinstance(int, object)) # True
print(isinstance(int_instance, object)) # True
print(isinstance(int, int)) # False
print(isinstance(int_instance, int)) # True

print(issubclass(str, object)) # True
print(issubclass(str_instance, object)) #Error
print(issubclass(str, str)) # True
print(issubclass(str_instance, int)) # Error
print(isinstance(str, object)) # True
print(isinstance(str_instance, object)) # True
print(isinstance(str, str)) # False
print(isinstance(str_instance, str)) #True
```

### 2.2 Type Meta-Class
```pyhton
print(isinstance(object, type)) # True
print(isinstance(type, object)) # True
print(issubclass(object, type)) # False
print(issubclass(type, object)) # True

print(issubclass(object, object)) # True
print(issubclass(object, object)) # True

print(type(object)) # <class 'type'>
print(type(type)) # <class 'type'>

print(isinstance(type, object)) # True
print(issubclass(object, type)) # False
print(type(str)) # <class 'type'>
print(type(int)) # <class 'type'>

int_instance = 13
print(isinstance(int_instance, type)) # False
print(issubclass(int_instance, type)) # Error
```

### 2.3 Overloading vs. Overriding
*Warning*: **In python, we have NO Overloading at all!** (Beacause of the \**args* and \**kwargs*)
- Overloading: Overloading occurs when two or more methods in one class have the same method name but different parameters.
- Overwriting: Overriding means having two methods with the same name and parameters but differernt definition; One of the methods is in the parent class and the other is in the child class.

### 2.4 Inheritance vs. Instantiation from Meta-Class
### 2.5 Gang of Three Methods
- \_\_new__
-	\_\_init__
-	\_\_call__

### 2.6 When to Define Meta-Class
### 2.7 Gang of Three Method Types!
- static methods
- object methods
- class methods

### 2.8 Design Patterns
- Structural
- Behavioral
- Creational

### 2.9 Singleton Design Pattern

---

## TA 1

---

### TA1.1 Method Resolution Order
### TA1.2 Factory Design Pattern
### TA1.3 Abstract Classes (_abc_ Module)

---

## Session 3

---

### 3.1 Observer Design Pattern
### 3.2 UML
### 3.3 BFS Algorithm for Graph Class of Previous Session
### 3.4 Coupling (and IOC) vs Cohesion
### 3.5 Abstract Class
### 3.6 Closure in Python
### 3.7 Linter in Text Editors
### 3.8 Abstract Classes Vs. Interfaces
### 3.9 Decorators
### 3.10 Decorators with Arguments

