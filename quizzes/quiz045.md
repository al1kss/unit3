# Quiz 045

## Code
```.py
class WordCounter:
    def __init__(self):
        self.output = {}

    def count_words(self, w):
        words = w.split()
        for word in words:
            if word in self.output:
                self.output[word] += 1
            else:
                self.output[word] = 1
        return self.output

x = WordCounter()
print(x.count_words("This is a sample text. It contains some words that will be counted."))

```

## Proof of work
<img width="1470" alt="Screenshot 2025-02-27 at 8 10 14" src="https://github.com/user-attachments/assets/2ecb7e43-3450-4459-99be-858d17a99061" />

## Paper Solution
![WhatsApp Image 2025-02-27 at 09 59 25](https://github.com/user-attachments/assets/76d37cca-d5c7-468b-b2dd-bb1d20fbaf6f)


### For my info
Where is it on PC
>Documents/Coding/CS Lessons/Quizzes/Unit 3/quiz045
