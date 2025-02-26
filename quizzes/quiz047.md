# Quiz 047

## Code
```.py
class CalorieCount:
    def __init__(self, limit):
        self.limit = limit
        self.intake = 0
        self.protein = 0

    def addMeal(self, intake, protein, carbs, fat):
        self.protein += protein
        self.intake += intake
        if self.intake > self.limit:
            return "Limit exceeded"
        return self.intake

    def getProteinPercentage(self) -> float:
        return (4*self.protein)/ self.intake

    def onTrack(self)-> bool:
        if self.intake <= self.limit:
            return True
        return False

sunday = CalorieCount(1500)

sunday.addMeal(716, 38, 38, 45)
sunday.addMeal(230, 16, 8, 16)
sunday.addMeal(568, 38, 50, 24)

print(sunday.onTrack()) #returns False
print(sunday.getProteinPercentage())
#returns 0.24

```

## Proof of work
<img width="1470" alt="Screenshot 2025-02-27 at 8 24 30" src="https://github.com/user-attachments/assets/5e0c4cfb-abe1-42dc-9906-3e8bfaca29c3" />

## Paper Solution


### For my info
Where is it on PC
>Documents/Coding/CS Lessons/Quizzes/Unit 3/quiz047
