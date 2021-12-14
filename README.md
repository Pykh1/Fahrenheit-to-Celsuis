# Fahrenheit-to-Celsuis
Produce a GUI that allows a user to enter Tempurature in fahrenheit and have it display the tempurature in Celsuis on click of button using Python TKINTER


from tkinter import *
def feh_to_cel():
    Fahrenheit=float(Fahrenheit_entry.get())
    celsuis=(Fahrenheit -32)*5/9
    display_celsuis_label["text"]=celsuis



my_window = Tk()

label_1=Label(my_window,text="enter Fahrenheit")
Fahrenheit_entry=Entry(my_window)
label_2=Label(my_window,text="display_celsuis")
display_celsuis_label =Label(my_window)
convert_button = Button(my_window,text="convert here",command=feh_to_cel)

label_1.grid(row=0,column=0)
Fahrenheit_entry.grid(row=0,column=1)
label_2.grid(row=1,column=0)
display_celsuis_label.grid(row=1,column=1)
convert_button.grid(row=2,column=0)

my_window.mainloop()
