# Quiz 036

## Code
```.py
from kivymd.app import MDApp

class quiz036(MDApp):
    def build(self):
        return
    def close(self):
        exit()
    def on_press(self):
        self.root.ids.my_screen_2.md_bg_color = "#000000"
        self.root.ids.my_screen_2.color = "#FFFFFF"
        self.root.ids.my_button.md_bg_color = "#1BA7DC"

t = quiz036()
t.run()
```
## KV Code
```.kv
MDScreen:

    size: 500, 500
    md_bg_color: "#FFFFFF"

    MDLabel:
        id: my_screen_2
        text: "Your Name"
        halign: "center"
        font_size: "58pt"
        pos_hint: {"center_x": .5, "center_y": .5}


    MDRaisedButton:
        id: my_button
        text: "Change!"
        md_bg_color: "#c1121f"
        on_press:
            app.on_press()

```
## Proof of work
<img width="814" alt="Screenshot 2025-01-29 at 23 31 00" src="https://github.com/user-attachments/assets/c53c47e4-943f-413c-97d9-5899d0fd632a" />
<img width="810" alt="Screenshot 2025-01-29 at 23 31 14" src="https://github.com/user-attachments/assets/d529e5ed-2d57-41d0-88f0-e933901bc9a2" />


### For my info
Where is it on PC
>Documents/Coding/CS Lessons/Quizzes/Unit 3/quiz036
