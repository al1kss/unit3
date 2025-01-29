# Quiz 037

## Code
```.py
from kivymd.app import MDApp

class quiz037(MDApp):
    def build(self):
        self.turn = "X"
        return

    def button_pressed(self, button):

        if button.text != "":
            return

        button.md_bg_color = "#015D66"
        button.text = self.turn
        if self.turn == "X":
            self.turn = "O"
            button.text_color = "#FF5733"
        else:
            self.turn = "X"
            button.text_color = "#FFC300"

        self.root.ids.turn.text = f"It's {self.turn}'s turn"

test = quiz037()
test.run()
```

## KV Code
```.kv
MDScreen:
    size: 300, 100
    md_bg_color: "#26242b"

    BoxLayout:
        size_hint: 1, .8
        orientation: "vertical"
        spacing: 10
        padding: 10
        pos_hint: {"center_x": .5, "center_y": .5}
        md_bg_color: "#0c1a1e"


        MDLabel:
            text: "Tic Tac Toe by Alikhan"
            font_style: "H4"
            halign: "center"
            size_hint_y: .1
            color: "#FFFFFF"
            padding: 10

        MDLabel:
            id: turn
            text: "It's X's turn"
            font_style: "H6"
            halign: "center"
            size_hint_y: .15
            color: "#FFFFFF"
            padding: 10





        GridLayout:
            cols: 3
            rows: 3
            spacing: 10
            size_hint: 1, .8

            MDFillRoundFlatButton:
                id: one
                text: ""
                md_bg_color: "#4f4d54"
                text_size: "30dp"
                size_hint: 1, 1
                on_press:
                    app.button_pressed(one)

            MDFillRoundFlatButton:
                id: two
                text: ""
                md_bg_color: "#4f4d54"
                text_size: "30dp"
                size_hint: 1, 1
                on_press:
                    app.button_pressed(two)

            MDFillRoundFlatButton:
                id: three
                text: ""
                md_bg_color: "#4f4d54"
                text_size: "30dp"
                size_hint: 1, 1
                on_press:
                    app.button_pressed(three)

            MDFillRoundFlatButton:
                id: four
                text: ""
                size_hint: 1, 1
                md_bg_color: "#4f4d54"
                text_size: "30dp"
                on_press:
                    app.button_pressed(four)

            MDFillRoundFlatButton:
                id: five
                text: ""
                size_hint: 1, 1
                md_bg_color: "#4f4d54"
                text_size: "30dp"
                on_press:
                    app.button_pressed(five)

            MDFillRoundFlatButton:
                id: six
                text: ""
                md_bg_color: "#4f4d54"
                size_hint: 1, 1
                text_size: "30dp"
                on_press:
                    app.button_pressed(six)

            MDFillRoundFlatButton:
                id: seven
                text: ""
                text_size: "30dp"
                md_bg_color: "#4f4d54"
                size_hint: 1, 1
                on_press:
                    app.button_pressed(seven)

            MDFillRoundFlatButton:
                id: eight
                text: ""
                text_size: "30dp"
                size_hint: 1, 1
                md_bg_color: "#4f4d54"
                on_press:
                    app.button_pressed(eight)

            MDFillRoundFlatButton:
                id: nine
                text: ""
                text_size: "30dp"
                md_bg_color: "#4f4d54"
                size_hint: 1, 1
                on_press:
                    app.button_pressed(nine)
```

## Proof of work
<img width="832" alt="Screenshot 2025-01-29 at 23 28 59" src="https://github.com/user-attachments/assets/7ccde49c-6b30-49ac-a41c-81cb9b7a1061" />
<img width="820" alt="Screenshot 2025-01-29 at 23 29 14" src="https://github.com/user-attachments/assets/fcaa82f9-ab0d-464d-bfa0-f875efc6c0de" />


### For my info
Where is it on PC
>Documents/Coding/CS Lessons/Quizzes/Unit 3/quiz037
