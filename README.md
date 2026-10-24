# teste-biblioteca-python

import tkinter as tk
from tkinter import messagebox

def mostrar_mensagem():
    messagebox.showinfo("Teste", "A biblioteca Tkinter está funcionando!")

janela = tk.Tk()
janela.title("Teste da biblioteca Tkinter")
janela.geometry("400x200")

titulo = tk.Label(
    janela,
    text="Teste da biblioteca Tkinter",
    font=("Arial", 14)
)
titulo.pack(pady=20)

botao = tk.Button(
    janela,
    text="Clique aqui",
    command=mostrar_mensagem
)
botao.pack()

janela.mainloop()
