# Quiz 032

## Code
```.py
class HumanResources:
    def __init__(self, name, occupation, age, phone):
        self.name = name
        self.occupation = occupation
        self.age = age
        self.phone = phone
        self.email = None
        self.nationality = None

    def set_email(self, email):
        self.email = email
        return "Successful!"

    def get_email(self):
        return self.email

    def set_nationality(self, nationality: str):
        self.nationality = nationality
        return "Successful!"

    def greeting(self)->str:
        return f"Hello {self.name}. I am {self.occupation}."
```

## Proof of work


### For my info
Where is it on PC
>Documents/Coding/CS Lessons/Quizzes/Unit 3/quiz032
