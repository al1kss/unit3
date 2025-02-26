# Quiz 048

## Code
```.py
from audioop import lin2adpcm


class Book:
    def __init__(self, title, author, isbn):
        self.title = title
        self.author = author
        self.isbn = isbn

    def display_info(self):
        return f"A {self.title} by {self.author}, ISBN: {self.isbn}"

class Library:
    def __init__(self):
        self.books = []

    def add_Books(self, other: Book):
        self.books.append(other)
        return self.books

    def show_books(self):
        output = ""
        for i in self.books:
            output += i.display_info() + "\n"
        return output

book1 = Book("godfather", "Mario Putho", "1234")
book2 = Book("The first teacher", "Chyngyz Aitmatov", "5678")
book3 = Book("1984", "George Orwell", "91011")

library = Library()
library.add_Books(book1)
library.add_Books(book2)
library.add_Books(book3)
print(library.show_books())
```

## Proof of work
<img width="1470" alt="Screenshot 2025-02-27 at 8 38 34" src="https://github.com/user-attachments/assets/1e0ea583-08b2-4846-9148-692b7194627e" />

## Paper Solution


### For my info
Where is it on PC
>Documents/Coding/CS Lessons/Quizzes/Unit 3/quiz048
