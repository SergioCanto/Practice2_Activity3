from grovepi import *
import time
import grovepi
import math
from grove_rgb_lcd import *
import random

sensor = 0
BOTON = 4

setText("Presiona el BOTON")
temp = grovepi.temp(sensor,'1.1')
setRGB(0,0,255) #RED
pinMode(BOTON,"INPUT")   

while True:
    button_status= digitalRead(BOTON)  
    if button_status:   
        temp = grovepi.temp(sensor,'1.1')
        print("temp =", temp)
        time.sleep(.5)
        setText("TEMP = " + str(int(temp)))
        setRGB(0,255,0)
        time.sleep(.5)
    else:
        setText("Presiona el boton")
        setRGB(255,0,0) 
        time.sleep(.5)
