from tkinter import *
import time
import webbrowser

root = Tk()

frameuser = Frame()
frameuser.grid()

def ENT(event):
    user = Entryuser.get()

    if(user == 'youtube'):
        webbrowser.open_new_tab("https://www.YouTube.com/")

    if(user == 'Youtube'):
        webbrowser.open_new_tab("https://www.YouTube.com/")

    if(user == 'YouTube'):
        webbrowser.open_new_tab("https://www.YouTube.com/")

    if(user == 'google'):
        webbrowser.open_new_tab("https://www.google.com/")

    if(user == 'Google'):
        webbrowser.open_new_tab("https://www.google.com/")

global Entryuser
Entryuser = Entry(root)
Entryuser.grid(row=0,column=0)

global Entryuseradd
Entryuseradd = Entry(root)
Entryuseradd.grid(row=2,column=0)

root.bind("<Return>",ENT)

root.mainloop()
