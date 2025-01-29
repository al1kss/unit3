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

### For my info
Where is it on PC
>Documents/Coding/CS Lessons/Quizzes/Unit 3/quiz036
