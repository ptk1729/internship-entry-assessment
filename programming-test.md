# Programming Test

This test was composed to create a general overview of your knowledge regarding general programming and how it fits with the needs in our lab. Please try to answer all questions using your own knowledge and in your own words. If you get stuck on one of the exercises, still try to give a short answer.

---

## Exercise 1

### Task
Write a program in the language of your choice where:

1. The iteration number (starting from 1), followed by a random number between 1 and 100, is printed 100 times.
2. After every 5 iterations, write an additional separator (e.g., `---`).
3. Write “Lucky number!” after every random number that is divisible by 7.

> Try to keep the procedure as short as possible.

Solution:
```python
import random

for i in range(1, 101):
    
    num = random.randint(1, 100)
    print(f"{i}: {num}", end='')
    
    if num % 7 == 0:
        print("  Lucky number!", end='')
    print()
    if i % 5 == 0:
        print("---")
```
---

## Exercise 2

### 1. **What is your understanding of the term “Design Patterns”?**  
   Solution:
#### A Design Pattern is
   - A description of a standard solution for
   - A standard design problem
   - In a certain context

### 2. **Explain the MVC Pattern**  
   - What does MVC stand for?  
   - Explain the pattern in detail.  
   - What are some use cases for this framework?
### Solution:

**What MVC stands for**
It’s short for **Model-View-Controller**.

**How it works, in plain terms**

* **Model**
  This is where your data lives—think of it as the part that stores things like user info, settings, or any business rules. It doesn’t care how it’s shown on screen or how people click around.
* **View**
  This is what people see: buttons, lists, charts, forms. You can have more than one view for the same data (like a table view and a graph view), and each one keeps itself up to date when the model changes.
* **Controller**
  This listens for what the user does—clicks, taps, typing—and then tells the model to change or tells the view to redraw. It’s the middleman that keeps the model and view from being too tightly linked.

Putting these three parts together means you can work on your data logic, your screen layout, and your user interactions separately. That makes it simpler to test, tweak, or swap out one piece without touching the others.

---

**MVC in action**

* **Web apps** like Ruby on Rails or ASP.NET MVC
* **Desktop interfaces** using toolkits such as Java Swing or Cocoa on macos
* **Mobile apps**, especially early iOS projects or many Android setups
* **Single-page web apps** with frameworks like Angular or Nextjs


### 3. **List three other design patterns**  
   - Provide names and details for three additional design patterns.
   - Explain how you have used those patterns in the past and how they have solved your problem  
   - Use diagrams to explain the design patterns.

---

## Exercise 3

### 1. **Implementation Task**  
   Based on the class diagram below, provide an implementation in any object-oriented programming language of your choice.
   
```mermaid
classDiagram

class A {
	# Name : string
	+ PrintName() void
}

<<abstract>> A

class B {
	- PrintName(message : string) void
}

class C {
	+ PrintName(message : string) void
}

D --|> A
B --|> A
C --|> B
```

### 2. **Key Questions**  
   - Are you able to directly create a new instance of `ObjectA`? Please explain your answer.  
   - Given an instance of `ObjectC`, are you able to call the method `PrintMessage` defined in `ObjectB`? Please explain your answer.  
   - Try to explain as many key features of object-oriented programming as you can find in this example.

---

## Exercise 4

### Maintaining and Expanding Software for Component Validation

This exercise focuses on strategies for working with existing code bases and ensuring the software remains maintainable as new features and requirements are introduced.

### 1. **Working with Existing Code**  
- How would you approach understanding and contributing to an existing code base with minimal disruption?  
- What practices would you follow to ensure your changes integrate well with the current structure?  

### 2. **Ensuring Maintainability**  
- What techniques would you use to keep the code base clean, modular, and easy to maintain as new features are added?  
- How would you handle code documentation and testing to support long-term maintainability?  

### 3. **Balancing Flexibility and Stability**  
- How would you design or refactor the software to make it flexible for future changes while ensuring the existing functionality remains stable?  
- Which design patterns or principles would you apply to achieve this balance
---
