# Basic-Calculator
The first application I designed in my way of learning python, calculator with only 4 functions(+,-,*,/)

import tkinter as tk
def sum():
    if number2.get().isdigit() and number2.get().isdigit() :
        n1=float(number1.get())
        n2=float(number2.get())
        Result.configure(text=str(n1+n2))

def subtraction():
    if number2.get().isdigit() and number2.get().isdigit() :
        n1=float(number1.get())
        n2=float(number2.get())
        Result.configure(text=str(n1-n2))

def multiplation():
    if number2.get().isdigit() and number2.get().isdigit() :
        n1=float(number1.get())
        n2=float(number2.get())
        Result.configure(text=str(n1*n2))

def division():
    if number2.get().isdigit() and number2.get().isdigit() :
        n1=float(number1.get())
        n2=float(number2.get())
        Result.configure(text=str(n1/n2))







window = tk.Tk()
window.title('Calculator')
screnwidth=window.winfo_screenwidth()//2-160
screnheight=window.winfo_screenheight()//2-150
window.geometry("320x300+{}+{}".format(screnwidth,screnheight))

Result=tk.Label(window, text ="result",font="courier 16 bold", width=30,justify="center")
Result.place(x=-50, y=20)
number1 = tk.Entry(window, font="courier 14 bold", width=15, justify="right")
number1.place (x=70, y=50)
number2 = tk.Entry(window, font="courier 14 bold", width=15, justify="right")
number2.place (x=70, y=80)

button1 =tk.Button(window, text ="+", font="courier 14 bold", width=10, command=sum)
button1.place(x=90, y=110)

button2 =tk.Button(window, text ="-", font="courier 14 bold", width=10, command=subtraction)
button2.place(x=90, y=150)

button3 =tk.Button(window, text ="*", font="courier 14 bold", width=10, command=multiplation)
button3.place(x=90, y=190)

button4 =tk.Button(window, text ="/", font="courier 14 bold", width=10, command=division)
button4.place(x=90, y=230)

number1.focus()





window.mainloop()
