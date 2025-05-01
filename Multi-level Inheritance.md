# Exp.No:24  
## Multi-level Inheritance

### AIM  
To write a Python program to get the name, age, and ID of a person and display them using multilevel inheritance.

### ALGORITHM

1. Define the `Person` class:
   - Inside the `Person` class, define the `__init__` method (constructor) with two parameters: `name` and `age`.
   - Inside the `__init__` method, assign the `name` to `self.name` and `age` to `self.age`.

2. Define the `PersonDetails` class that inherits from the `Person` class:
   - Inside the `PersonDetails` class, define the `__init__` method (constructor) with three parameters: `name`, `age`, and `person_id`.
   - Inside the `__init__` method, call the `__init__` method of the `Person` class using `super()` to initialize `name` and `age`.
   - Assign `person_id` to `self.person_id`.

3. Define the `DisplayDetails` class that inherits from the `PersonDetails` class:
   - Inside the `DisplayDetails` class, define the `__init__` method (constructor) with three parameters: `name`, `age`, and `person_id`.
   - Inside the `__init__` method, call the `__init__` method of the `PersonDetails` class using `super()` to initialize `name`, `age`, and `person_id`.

4. Inside the `DisplayDetails` class, define the `show_details` method:
   - Inside the `show_details` method, return a formatted string with `self.name`, `self.age`, and `self.person_id`.

5. Prompt the user to enter `name` (string), `age` (integer), and `person_id` (integer).

6. Create an instance `person` of the `DisplayDetails` class, passing `name`, `age`, and `person_id` to the constructor.

7. Call the `show_details` method on the `person` object and print the result.

8. Terminate the program.


### PROGRAM

```
# Reg.No-212223050048
# Name-SIBIRAJI M
# Write your code here
class Person:
    def __init__(self,name):
        self.name=name
class Employee(Person):
    def __init__(self,name,age):
        super().__init__(name)
        self.age=age
class Id(Employee):
    def __init__(self,name,age,id):
        super().__init__(name,age)
        self.id=id
    def display(self):
        print(f"{self.name} {self.age} {self.id}")

def main():
    name=input()
    age=int(input())
    id=int(input())
    person=Id(name,age,id)
    person.display()
main()
```

### OUTPUT
![image](https://github.com/user-attachments/assets/73f8428e-e025-46f8-b349-ebb4113757dd)

### RESULT
Thus the Python program to get the name, age, and ID of a person and display them using multilevel inheritance. is executed successfully.
