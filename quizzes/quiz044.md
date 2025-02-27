# Quiz 044

## Code
```.py
class rainDrops:
    def __init__(self):
        self.output = ""

    def pour(self, n)->str:
        if n % 3 == 0:
            self.output += "Pling"
        if n % 5 == 0:
            self.output += "Plang"
        if n % 7 == 0:
            self.output += "Plong"
        if self.output == "":
            return str(n)
        return self.output

rain = rainDrops()
print(rain.pour(28))
rain1 = rainDrops()
print(rain1.pour(30))
rain2 = rainDrops()
print(rain2.pour(34))
```

## Proof of work
<img width="1470" alt="Screenshot 2025-02-26 at 21 16 43" src="https://github.com/user-attachments/assets/eb4fe2dd-bcfe-4245-a012-0e3548df1cda" />

## Paper Solution
![WhatsApp Image 2025-02-27 at 11 11 19 (1)](https://github.com/user-attachments/assets/00a79872-1de5-4466-9cd0-04198702dc86)


### For my info
Where is it on PC
>Documents/Coding/CS Lessons/Quizzes/Unit 3/quiz044
