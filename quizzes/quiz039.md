# Quiz 039

## Code
```.py
import sqlite3

haiku = """Code flows like a stream 
Algorithms guide its way
In silence, it solves"""

con = sqlite3.connect("haiku.db")
cursor = con.cursor()

#Create Database with table Words
for word in haiku.split():
    query_create_table = f"""
    create table if not exists Words(
        id INTEGER PRIMARY KEY,
        len INTEGER not null,
        word TEXT UNIQUE
    );
    """
    cursor.execute(query_create_table)
    con.commit()

    insert = f"INSERT into Words(len, word) values ('{len(word)}','{word}');"
    cursor.execute(insert)
    con.commit()

#querying
output = cursor.execute("SELECT AVG(len) from Words;")
result = output.fetchall() #fetchall means all the results from the query
print("Average length:", result)

con.close()

```

## Proof of work
<img width="313" alt="Screenshot 2025-01-29 at 23 27 39" src="https://github.com/user-attachments/assets/3409245b-5a86-4be4-b5fc-721aa63d8bea" />


### For my info
Where is it on PC
>Documents/Coding/CS Lessons/Quizzes/Unit 3/quiz039
