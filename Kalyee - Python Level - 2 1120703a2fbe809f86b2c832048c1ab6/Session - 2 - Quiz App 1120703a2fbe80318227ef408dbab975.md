# Session - 2 - Quiz App

![image.png](Session%20-%202%20-%20Quiz%20App%201120703a2fbe80318227ef408dbab975/image.png)

```python
import tkinter as tk 

window = tk.Tk() 

window.geometry("300x300")
window.title("Quiz app")

currentQuestion = -1

questions = [
    {
        "question":"What is this fruit ? ",
        "options" : ["apple" , "orange","banana" , "pineapple"],
        "correct": "orange"
    },
    {
        "question":"What is this vegitable ? ",
        "options" : ["bringle" , "ladyfinger", "califlower" , "soya"],
        "correct": "apple"

    },
    {
        "question":"What is this country? ",
        "options" : ["Japan" , "India" , "USA", "Russia"],
        "correct": "India"

    },
    {
        "question":"What is this color? ",
        "options" : ["orange" , "red", "pink" , "violet"],
        "correct": "red"

    },
]

def updateQuestion():
    global currentQuestion
    currentQuestion += 1 

    questionLabel = tk.Label(text=questions[currentQuestion]["question"])
    questionLabel.grid(row = 0  , column =1)

    for i in range(4) : 
        optionLabel = tk.Label(text = questions[currentQuestion]["options"][i] , width = 10 )
        optionLabel.grid(row= i + 1 , column = 2) 
        radioButton = tk.Radiobutton( value = i)
        radioButton.grid(row = i + 1  , column =1)

nextButton = tk.Button(text = "Next" , command = updateQuestion)
nextButton.grid(row = 10 , column = 2 )

previousButton = tk.Button(text = "Previous" )
previousButton.grid(row = 10 , column = 1 )

window.mainloop()
```