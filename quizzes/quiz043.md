# Quiz 043

## Code
```.py
class palNum:
    def __init__(self):
        self.output = []

    def get_pal_list(self, num_down, num_up):
        for i in range(num_down, num_up+1):
            if str(i) == str(i)[::-1]:
                self.output.append(i)
        return self.output

num = palNum()
print(num.get_pal_list(1, 9))
print(num.get_pal_list(10, 199))

```

## Proof of work
<img width="1470" alt="Screenshot 2025-02-26 at 21 09 10" src="https://github.com/user-attachments/assets/98351516-3178-429d-9fea-83818748f019" />

## Paper Solution
![WhatsApp Image 2025-02-26 at 21 09 39](https://github.com/user-attachments/assets/1dad56f1-2dd1-408d-bbc2-db1f08ced0a9)


### For my info
Where is it on PC
>Documents/Coding/CS Lessons/Quizzes/Unit 3/quiz043
