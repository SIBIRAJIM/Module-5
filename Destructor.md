# Exp.No:22  
## Destructor

### AIM  
To create a Python class `Student` with a destructor.

### ALGORITHM

1. Begin the program.  
2. Define the `student` class.  
3. Inside the `student` class, define the `__init__` method (constructor) and the `__del__` method (destructor).  
4. Create an object `s2` of the `student` class. When the object `s2` is created, the `__init__` method is called, and its print statements are executed.  
5. Use the `del` statement to delete the object `s2`. This triggers the `__del__` method (destructor), and the respective print statements are executed.  
6. Terminate the program.


### PROGRAM

```
# Reg.No-212223050048
# Name-SIBIRAJI M
# Write your code here
class Student:

    # constructor
    def __init__(self, name):
        print('Inside Constructor')
        self.name = name
        print('Object initialized')

    def show(self):
        print('Hello, my name is', self.name)

    # destructor
    def __del__(self):
        print("Inside destructor")
        print("Object destroyed")

# create object
s1 = Student('Emma')
s1.show()

# delete object
del s1
```

### OUTPUT
![image](https://github.com/user-attachments/assets/27a0b8e2-8813-442f-8180-d8785a1e5ab9)

### RESULT
Thus the Python class `Student` with a destructor is executed successfully.
