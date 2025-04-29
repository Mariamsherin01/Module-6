# Exp.No:30  
## POLYMORPHISM

---

### AIM  
To implement polymorphism in Python using user-defined methods area() and perimeter() in Square and Circle classes.

---

### ALGORITHM

1.Define two classes Square and Circle, each with methods area() and perimeter().

2.In each class, implement area() and perimeter() based on the shape's formulas.

3.Create objects for both classes with user-provided values.

4.Call area() and perimeter() on each object to demonstrate polymorphism.

---

### PROGRAM

```
import math

class Square:
    def __init__(self, side):
        self.side = side

    def perimeter(self):
        print("Perimeter computed for square: ", 4 * self.side)

    def area(self):
        print("Area computed for square: ", self.side * self.side)

class Circle:
    def __init__(self, radius):
        self.radius = radius

    def perimeter(self):
        print("Perimeter computed for Circle: ", 2 * math.pi * self.radius)

    def area(self):
        print("Area computed for Circle: ", math.pi * self.radius * self.radius)

# Input
radius = int(input())
side = int(input())

# Objects
square = Square(side)
circle = Circle(radius)

# Output
square.perimeter()
square.area()
circle.perimeter()
circle.area()

```

### OUTPUT
![image](https://github.com/user-attachments/assets/fb40008b-33db-40ee-aba9-ff78c0c375ce)


### RESULT
Thus, To implement polymorphism in Python using user-defined methods area() and perimeter() in Square and Circle classes was implemented and executed successfully.
