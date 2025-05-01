# Exp.No:21  
## Constructors - Parameterized Constructor


### AIM  
To write a python code to implement a parameterised constructor that will initialize the name and age of the student and print the details using user defined function.

### ALGORITHM

1. Begin the program.  
2. Define a `person` class.  
3. The `person` class should have a parameterized `__init__` method that accepts two parameters: `name` and `age`.  
4. Inside the `__init__` method, assign the `name` to `self.name` and the `userid` to `self.age`.  
5. Print the `self.age`.  
6. Prompt the user to enter their `name` (string) and `age`.  
7. Create an instance `s1` of the `person` class by passing the entered `name` and `age` to the constructor.  
8. Terminate the program.


### PROGRAM

```
# Reg.No-212223050048
# Name-SIBIRAJI M
# Write your code here
class Student:
    def __init__(self,name,age):
        self.name=name
        self.age=age
    def Print(self):
        # printing the name and age
        print("Student name is :", self.name)
        print("Student age is : ", self.age)
# creating object of type Student
name=input()
age=int(input())

student = Student(name,age)
# calling the Print method
student.Print() 
```

### OUTPUT
![image](https://github.com/user-attachments/assets/7067ccca-c6b1-449b-83f1-d39aef6939eb)

### RESULT
Thus the python code to implement a parameterised constructor that will initialize the name and age of the student and print the details using user defined function is executed successfully.
