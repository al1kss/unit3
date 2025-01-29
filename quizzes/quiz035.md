# Quiz 035

## Code
```.py
class Person():
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def get_name(self):
        return self.name

    def get_age(self):
        return self.age

class Student(Person):
    def __init__(self, name, age, grade):
        super().__init__(name, age)
        self.grade = grade

```

## Part B

### For my info
Where is it on PC
>Documents/Coding/CS Lessons/Quizzes/Unit 3/quiz035
