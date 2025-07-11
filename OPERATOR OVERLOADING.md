# Exp.No:27  
## Operator Overloading

---

### AIM  
To write a Python program to perform division of two complex numbers using the binary '/' operator overloading. Class name: `Complex`, where the objects `Ob1 = Complex(10, 21)` and `Ob2 = Complex(2, 3)` represent complex numbers.

---

### ALGORITHM

1. **Start the Program.**
2. **Define the Complex class**:
   - Define the constructor `__init__()` to accept two parameters: `real` and `imag` (representing the real and imaginary parts of the complex number).
   - Assign these values to `self.real` and `self.imag` respectively.
3. **Define the `__truediv__()` method** to perform the division of two complex numbers:
   - Calculate the real part of the result as the division of `self.real` by `other.real`.
   - Calculate the imaginary part of the result as the division of `self.imag` by `other.imag`.
   - Return a new Complex object with the calculated real and imaginary parts.
4. **Define the `__repr__()` method** to represent the complex number as a string.
   - Return a string formatted to display the real and imaginary parts with one decimal place using `f"{self.real:.1f}, {self.imag:.1f}"`.
5. **Create two objects of the Complex class**:
   - `Ob1 = Complex(10, 21)` represents the complex number `10 + 21i`.
   - `Ob2 = Complex(2, 3)` represents the complex number `2 + 3i`.
6. **Perform the division operation**: Use the `/` operator to divide `Ob1` by `Ob2`. This will call the `__truediv__()` method.
7. **Print the result**: Print the result of the division, which will be formatted by the `__repr__()` method.
8. **End the Program.**

---

### PROGRAM

```
class complex:
    def __init__(self, real, imag):
        self.real = real
        self.imag = imag

    def __add__(self, other):
        # Complex division: (a + bi) / (c + di)
        a, b = self.real, self.imag
        c, d = other.real, other.imag
        denominator = c**2 + d**2
        real_part = (a*c + b*d) / denominator
        imag_part = (b*c - a*d) / denominator
        return (real_part, imag_part)

# Create objects
Ob1 = complex(10, 21)
Ob2 = complex(2, 3)

# Perform division using overloaded '+'
result = Ob1 + Ob2

# Display result
print(result)

```

### OUTPUT
![image](https://github.com/user-attachments/assets/b10ce8cc-46cc-489d-a9bd-d026760f4986)


### RESULT
Thus, The Python program to perform division of two complex numbers using the binary '/' operator overloading was implemented and executed successfully.
