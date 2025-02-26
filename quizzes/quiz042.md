# Quiz 042

## Code
```.py
import sqlite3

from secure_password import encrypt_password
from secure_password import check_password
from my_lib import DatabaseManager

x = DatabaseManager("bitcoin_exchange.db")
result = x.search("SELECT * from ledger;") #fetchall means all the results from the query
x.close()

for row in result:
    id, sender_id, receiver_id, amount, signature = row
    string_hash = f"id {id},sender_id {sender_id},receiver_ids {receiver_id},amount {amount}"
    print(signature)
    if check_password(user_password=string_hash, hashed_password=signature):
        print("TX is correct")
    else:
        print("TX is bad")
```

## Proof of work
<img width="1470" alt="Screenshot 2025-02-26 at 20 50 22" src="https://github.com/user-attachments/assets/d18a6b6e-9ec6-4414-b972-525bf3a95689" />

### For my info
Where is it on PC
>Documents/Coding/CS Lessons/Quizzes/Unit 3/quiz042
