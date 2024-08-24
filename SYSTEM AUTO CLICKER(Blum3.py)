from pyautogui import *
import pyautogui
import time as t
import keyboard
import random
import win32api, win32con

t.sleep(2)

#colour of center (205, 220,   0)

def click(x,y):
    win32api.SetCursorPos((x,y))
    win32api.mouse_event(win32con.MOUSEEVENTF_LEFTDOWN,0,0)
    win32api.mouse_event(win32con.MOUSEEVENTF_LEFTUP,0,0)

while keyboard.is_pressed('q') == False:
    pic = pyautogui.screenshot(region=(230,0,450,750))
    width, height = pic.size

    for x in range(0,width,5):
        for y in range(0,height,5):
            r,g,b = pic.getpixel((x,y))

            if (g in range(220,225)) & (r in range(200,206)):
                click(x+230, y+0)
                break
