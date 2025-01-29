# Quiz 038

## Code
```.py
from kivymd.app import MDApp
from kivymd.uix.screen import MDScreen


class Mystery(MDScreen):
    def next(self):
        self.parent.current = "MysteryPageA"

class MysteryPageA(MDScreen):
    def next(self):
        self.parent.current = "MysteryPageB"


class MysteryPageB(MDScreen):
    def back(self):
        self.parent.current = "MysteryPageA"


class quiz038(MDApp):
    def build(self):
        return

t = quiz038()
t.run()
```

## KV Code
```.kv
ScreenManager:
    id: scr_manager
    Mystery:
        name: "Mystery"
    MysteryPageA:
        name: "MysteryPageA"
    MysteryPageB:
        name: "MysteryPageB"

<Mystery>
    MDCard:
        orientation: "vertical"
        size_hint: .8, .8
        pos_hint: {"center_x": .5, "center_y": .5}
        radius: 30, 0, 30, 0 #top, left, bottom, right
        md_bg_color: "#ffb703"

        MDLabel:
            text: "Its first page"
            font_style: "H4"
            halign: "center"
            size_hint: 1, .1
            color: "#FFFFFF"

        MDRaisedButton:
            size_hint: .5, .1
            pos_hint: {"center_x": .75}
            text: "Next"
            md_bg_color: "#e63946"
            on_press:
                root.next()

<MysteryPageA>
    MDCard:
        orientation: "vertical"
        size_hint: .8, .8
        pos_hint: {"center_x": .5, "center_y": .5}
        radius: 30, 0, 30, 0 #top, left, bottom, right
        md_bg_color: "#DCC982"

        MDLabel:
            id: mystery_page_b
            text: "This is mystery page B you pressed the button"
            font_style: "H4"
            halign: "center"
            size_hint: 1, .1
            color: "#FFFFFF"

        MDRaisedButton:
            size_hint: .5, .1
            pos_hint: {"center_x": .75}
            text: "Next"
            md_bg_color: "#e63946"
            on_press:
                root.next()


<MysteryPageB>
    MDCard:
        orientation: "vertical"
        size_hint: .8, .8
        pos_hint: {"center_x": .5, "center_y": .5}
        radius: 30, 0, 30, 0 #top, left, bottom, right
        md_bg_color: "#C2D37D"

        MDLabel:
            text: "This is mystery page C you pressed the button"
            font_style: "H4"
            halign: "center"
            size_hint: 1, .1
            color: "#FFFFFF"

        MDRaisedButton:
            size_hint: .5, .1
            pos_hint: {"center_x": .75}
            text: "Back"
            md_bg_color: "#4E8484"
            on_press:
                root.back()
```

## Proof of Work
<img width="836" alt="Screenshot 2025-01-29 at 23 25 24" src="https://github.com/user-attachments/assets/f23a187b-b1e6-4614-9563-b808d8220fc3" />
<img width="905" alt="Screenshot 2025-01-29 at 23 24 58" src="https://github.com/user-attachments/assets/060d78f2-e8da-4740-915f-c717bd8193ec" />
<img width="841" alt="Screenshot 2025-01-29 at 23 25 11" src="https://github.com/user-attachments/assets/4c307277-fd40-49f7-ba7e-c13fa5aa2be7" />



### For my info
Where is it on PC
>Documents/Coding/CS Lessons/Quizzes/Unit 3/quiz038
