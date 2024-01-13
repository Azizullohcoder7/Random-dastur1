# Random-dastur1
import tkinter as tk
from tkinter import ttk
import random

def generate_random_name():
    names = []
    random_name = random.choice(names)
    result_label["text"] = f"Tasodifiy Ism: {random_name}"

# GUI ni yaratish
app = tk.Tk()
app.title("Tasodifiy Ism Generator")

# Interfeys elementlari
generate_button = ttk.Button(app, text="Tasodifiy Ism Tanlash", command=generate_random_name)
result_label = ttk.Label(app, text="Tasodifiy Ism: ")

# Elementlarni joylash
generate_button.pack(pady=10)
result_label.pack(pady=10)

# Dasturni ishga tushirish
app.mainloop()
