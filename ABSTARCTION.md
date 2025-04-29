# Exp.No:28  
## Abstraction

---

### AIM  
To write a Python program to define the abstract base class named `Polygon` and also define the abstract method. This base class is inherited by various subclasses. Implement the abstract method in each subclass. Create objects of the subclasses and invoke the `sides()` method.

---

### ALGORITHM

1. **Start the Program.**
2. **Import the ABC class** from the `abc` module to implement abstraction.
3. **Define the abstract base class Polygon**:
   - Inherit from `ABC` (Abstract Base Class).
   - Define an abstract method `sides()` with no implementation.
4. **Define the Triangle class** that inherits from `Polygon`:
   - Implement the `sides()` method to print `"Triangle has 3 sides"`.
5. **Define the Pentagon class** that inherits from `Polygon`:
   - Implement the `sides()` method to print `"Pentagon has 5 sides"`.
6. **Define the Hexagon class** that inherits from `Polygon`:
   - Implement the `sides()` method to print `"Hexagon has 6 sides"`.
7. **Define the Square class** that inherits from `Polygon`:
   - Implement the `sides()` method to print `"I have 4 sides"`.
8. **Create an object `t` of the Triangle class** and call the `sides()` method to print the number of sides.
9. **Create an object `s` of the Square class** and call the `sides()` method to print the number of sides.
10. **Create an object `p` of the Pentagon class** and call the `sides()` method to print the number of sides.
11. **Create an object `k` of the Hexagon class** and call the `sides()` method to print the number of sides.
12. **End the Program.**

---

### PROGRAM

```
from abc import ABC, abstractmethod

# Define the abstract base class
class Polygon(ABC):
    @abstractmethod
    def sides(self):
        pass

# Define the subclass for Triangle
class Triangle(Polygon):
    def sides(self):
        print("Triangle has 3 sides")

# Define the subclass for Square (I have 4 sides)
class Square(Polygon):
    def sides(self):
        print("I have 4 sides")

# Define the subclass for Pentagon
class Pentagon(Polygon):
    def sides(self):
        print("Pentagon has 5 sides")

# Define the subclass for Hexagon
class Hexagon(Polygon):
    def sides(self):
        print("Hexagon has 6 sides")

# Create objects of the subclasses and invoke the sides() method
triangle = Triangle()
square = Square()
pentagon = Pentagon()
hexagon = Hexagon()

triangle.sides()
square.sides()
pentagon.sides()
hexagon.sides()


```

### OUTPUT
![image](https://github.com/user-attachments/assets/86a1ca7f-14d1-4140-9951-e5227aa4f170)


### RESULT
Thus, The Python program to define the abstract base class named `Polygon` and also define the abstract method. This base class is inherited by various subclasses was implemented and executed successfully.
