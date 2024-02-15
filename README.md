# relay_setup_anpr

#How to interface relay with raspberry pi to switch AC devices

https://kitflix.com/how-to-interface-relay-with-raspberrypi/
https://www.youtube.com/watch?v=cn5oD02fnok&t=113s&ab_channel=Kitflix


led1 = 21 #GPIO pin to connect to relay
import RPi.GPIO as GPIO
import time
GPIO.setmode(GPIO.BCM)
GPIO.setup(led1, GPIO.OUT)
while True:
    GPIO.output(led1, True)    
    time.sleep(2)
    GPIO.output(led1, False)
    time.sleep(2)
#use port no 3 ,1,2 instead of port no given in this video 


