# Quiz 046

## Code
```.py
class Citizen:
    def __init__(self, name, city, status):
        self.name = name
        self.city = city
        self.status = status

    def getName(self):
        return self.name
    def getCity(self):
        return self.city
    def getStatus(self):
        return self.status

class Employee(Citizen):
    def __init__(self, name, city, status, salary):
        super().__init__(name, city, status)
        self.salary = salary

    def getSalary(self):
        return self.salary

class partTimeEmployee(Employee):
    def __init__(self, name, city, status, salary, hours, member):
        super().__init__(name, city, status, salary)
        self.hours = hours
        self.member = member

    def getMember(self):
        return self.member
```

## Proof of work
<img width="1470" alt="Screenshot 2025-02-27 at 8 16 04" src="https://github.com/user-attachments/assets/63116eff-0f19-4414-aea3-82147d68a3ca" />

## Paper Solution
![WhatsApp Image 2025-02-27 at 11 11 19](https://github.com/user-attachments/assets/d09a4d17-6bc5-4433-95f9-4de650cb0e6b)


### For my info
Where is it on PC
>Documents/Coding/CS Lessons/Quizzes/Unit 3/quiz046
