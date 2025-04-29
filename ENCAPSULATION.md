# Exp.No:29  
## Encapsulation

---

### AIM  
To add getter and setter methods to a class to access and modify private variables.

---

### ALGORITHM

1.Start the program.

2.Define a class named Class1Students.

3.Inside the __init__() constructor:

4.Declare two private instance variables __name and __age.

5.Initialize them using the values passed as arguments.

6.Define the method speak():

7.Print the name and age in a formatted string.

8.Define a getter method get_name():

9.Return the private variable __name.

10.Define a setter method set_name(name):

11.Update the private variable __name with the new value.

12.Define a getter method get_age():

13.Return the private variable __age.

14.Define a setter method set_age(age):

15.Update the private variable __age with the new value.

16.Create an object of the class Class1Students with initial values for name and age.

17.Call the speak() method to display initial values.

18.Use set_name() and set_age() to update the values.

19.Call the speak() method again to display the updated values.

20.End the program.

---

### PROGRAM

```
class Class1Students:
    def __init__(self, name, age):
        self.__name = name
        self.__age = age

    def speak(self):
        print(f"my name is {self.__name}, and I am {self.__age} years old.")

    # Getter for name
    def get_name(self):
        return self.__name

    # Setter for name
    def set_name(self, name):
        self.__name = name

    # Getter for age
    def get_age(self):
        return self.__age

    # Setter for age
    def set_age(self, age):
        self.__age = age

# Create object
student = Class1Students("Michael", 40)
student.speak()

# Use setter methods to update values
student.set_name("John")
student.set_age(25)

# Display updated values
student.speak()



```

### OUTPUT

![image](https://github.com/user-attachments/assets/b3feeb2e-beb9-47e5-84d3-3ae56124d830)

### RESULT
Thus,  To add getter and setter methods to a class to access and modify private variables was implemented and executed successfully.

