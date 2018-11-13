# ProyectoClima
Proyecto Clima
import numpy as np
import openpyxl
import matplotlib
matplotlib.use('TkAgg')
from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
import tkinter
import matplotlib.pyplot as plt


Ventana=tkinter.Tk()
def graphic():
    x=[1,2,3,4,5]
    y=x
    plt.plot(x,y)
    fig.canvas.draw()
fig = plt.figure()
FIGURE= FigureCanvasTkAgg(fig, master=Ventana)
FIGURE.get_tk_widget().grid(row=0, column=0)


Ventana.title("ClimatGraphic")
Ventana.geometry('380x300')
Ventana.configure(background='blue')
tkinter.Button(Ventana, text="graficar",command = graphic).grid(row=1, column=0)

Ventana.mainloop()
