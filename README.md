# 🎲 Dice Roller in Python

This is a simple dice rolling simulator made using Python, NumPy and Colorama.

## 🔧 Features
- Colorful terminal output using Colorama
- Random dice numbers using NumPy
- Loop-based interaction

## ▶️ Run the Script
```bash
python dice_roller.py


import time 
import numpy as np 
from colorama import Fore, init 

init(autoreset=True)

while True:
    A = input("Press 1 to roll the dice (or type 'exit' to quit): ")

    if A == "1":
        print(Fore.RED + "🎲 Dice is rolling...")
        time.sleep(1)
        dice = np.random.randint(1, 7)
        print(Fore.CYAN + f"You got: {dice}")

    elif A == "exit":
        print(Fore.YELLOW + "Exiting the game...")
        break

    else:
        print(Fore.RED + "Invalid input. Try again.")

# Made by: CZ ⚡

#RUN THE GAME AND ENJOY ⚡