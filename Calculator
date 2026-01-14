from tkinter import *
from tkinter import ttk
from ttkthemes import ThemedTk

window = ThemedTk(theme="aquativo")
window.title("Calculator by Vaggos")
window.geometry("350x270")
window.resizable(False, False)

result=""

def press(num):
    global result
    result=result+str(num)
    if result == "67":
        equation.set("Are you Serious Right Now?")
        result = ""
    else:
        equation.set(result)

def equalpress():
    global result
    try:
        total = str(eval(result))
        if total == "67":
            equation.set("Are you Serious Right Now?")
            result = ""
        else:
            equation.set(total)
            result = total
    except:
        equation.set('error')
        result=""

equation=StringVar()

def clear():
    global result
    result=""
    equation.set("")

txt = ttk.Entry(window, width=25, font=("Tahoma", 15), textvariable=equation, justify="right")
txt.grid(columnspan=5, padx=5, pady=8, ipady=6)

button_width = 11
button_pad = 4

btn = ttk.Button(window, text="1", width=button_width, padding=button_pad, command=lambda:press(1))
btn.grid(row=1, column=0)
btn = ttk.Button(window, text="2", width=button_width, padding=button_pad, command=lambda:press(2))
btn.grid(row=1, column=1)
btn = ttk.Button(window, text="3", width=button_width, padding=button_pad, command=lambda:press(3))
btn.grid(row=1, column=2)
btn = ttk.Button(window, text="+", width=button_width, padding=button_pad, command=lambda:press("+"))
btn.grid(row=1, column=3)
btn = ttk.Button(window, text="4", width=button_width, padding=button_pad, command=lambda:press(4))
btn.grid(row=2, column=0)
btn = ttk.Button(window, text="5", width=button_width, padding=button_pad, command=lambda:press(5))
btn.grid(row=2, column=1)
btn = ttk.Button(window, text="6", width=button_width, padding=button_pad, command=lambda:press(6))
btn.grid(row=2, column=2)
btn = ttk.Button(window, text="-", width=button_width, padding=button_pad, command=lambda:press("-"))
btn.grid(row=2, column=3)
btn = ttk.Button(window, text="*", width=button_width, padding=button_pad, command=lambda:press("*"))
btn.grid(row=3, column=3)
btn = ttk.Button(window, text="7", width=button_width, padding=button_pad, command=lambda:press(7))
btn.grid(row=3, column=1)
btn = ttk.Button(window, text="8", width=button_width, padding=button_pad, command=lambda:press(8))
btn.grid(row=3, column=2)
btn = ttk.Button(window, text="9", width=button_width, padding=button_pad, command=lambda:press(9))
btn.grid(row=3, column=0)
btn = ttk.Button(window, text="=", width=button_width, padding=button_pad, command=equalpress)
btn.grid(row=4, column=0)
btn = ttk.Button(window, text="0", width=button_width, padding=button_pad, command=lambda:press(0))
btn.grid(row=4, column=1)
btn = ttk.Button(window, text="Clear", width=button_width, padding=button_pad, command=clear)
btn.grid(row=4, column=2)
btn = ttk.Button(window, text="%", width=button_width, padding=button_pad, command=lambda:press("%"))
btn.grid(row=4, column=3)
btn = ttk.Button(window, text="/", width=button_width, padding=button_pad, command=lambda:press("/"))
btn.grid(row=5, column=0)
btn = ttk.Button(window, text=".", width=button_width, padding=button_pad, command=lambda:press("."))
btn.grid(row=5, column=1)
btn = ttk.Button(window, text="(", width=button_width, padding=button_pad, command=lambda:press("("))
btn.grid(row=5, column=2)
btn = ttk.Button(window, text=")", width=button_width, padding=button_pad, command=lambda:press(")"))
btn.grid(row=5, column=3)
btn = ttk.Button(window, text="**", width=button_width, padding=button_pad, command=lambda:press("**"))
btn.grid(row=6, column=0)

window.mainloop()
