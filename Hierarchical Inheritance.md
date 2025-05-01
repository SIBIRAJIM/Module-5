# Exp.No:25  
## Hierarchical Inheritance


### AIM  
To write a Python program to get the employee and patient details and display them using hierarchical inheritance. Create a parent (base) class named `Details` and two child (derived) classes named `Employee` and `Patient`.


### ALGORITHM

1. **Begin the program.**
2. **Create a class Details** with an `__init__` method to initialize three attributes: `id`, `name`, and `gender`.
3. **Define a method display_details()** to print the values of `id`, `name`, and `gender`.
4. **Create a class Employee** that inherits from the `Details` class. 
   - Add two additional attributes: `company` and `department`.
   - Override the `display_details()` method to print the employee-specific attributes (`company` and `department`) along with the inherited details.
5. **Create a class Patient** that also inherits from the `Details` class. 
   - Add two additional attributes: `hospital` and `department`.
   - Override the `display_details()` method to print the doctor-specific attributes (`hospital` and `department`) along with the inherited details.
6. **Accept input** for employee and doctor details.
7. **Create objects of Employee and Patient** using the input.
8. **Call the `display_details()` method** for both objects to print the details.
9. **Terminate the program.**


### PROGRAM
```
# Reg.No-212223050048
# Name-SIBIRAJI M
# Write your code here
class Details:
    def __init__(self,id,name,gender):
        self.id=id
        self.name=name
        self.gender=gender

class Employee(Details):
    def __init__(self,id,name,gender,company,dept):
        super().__init__(id,name,gender)
        self.company=company
        self.dept=dept
    def display(self):
        print(f"Employee Object")
        print(f"Id:  {self.id}")
        print(f"Name:  {self.name}")
        print(f"Gender:  {self.gender}")
        print(f"Company:  {self.company}")
        print(f"Department:  {self.dept}")
        
class Patient(Details):
    def __init__(self,id,name,gender,hospital,dept):
        super().__init__(id,name,gender)
        self.hospital=hospital
        self.dept=dept
    def display(self):
        print(f"Patient Object")
        print(f"Id:  {self.id}")
        print(f"Name:  {self.name}")
        print(f"Gender:  {self.gender}")
        print(f"Hospital:  {self.hospital}")
        print(f"Department:  {self.dept}")
        
def main():
    emp_id=int(input())
    emp_name=input()
    emp_gender=input()
    emp_company=input()
    emp_dept=input()
    employee=Employee(emp_id,emp_name,emp_gender,emp_company,emp_dept)
    employee.display()
    pat_id=int(input())
    pat_name=input()
    pat_gender=input()
    pat_hospital=input()
    pat_dept=input()
    patient=Patient(pat_id,pat_name,pat_gender,pat_hospital,pat_dept)
    print(" ")
    patient.display()
main()
    
```

### OUTPUT  
![image](https://github.com/user-attachments/assets/67b7dd29-c3bb-4e31-b918-43d63b9559e8)

### RESULT
Thus the Python program to get the employee and patient details and display them using hierarchical inheritance. Create a parent (base) class named `Details` and two child (derived) classes named `Employee` and `Patient` is executed successfully.
