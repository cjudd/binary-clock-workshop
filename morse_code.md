# Morse Code

This is a lab intended to test your ability to control LEDs and look up documentation. In this lab, you will create a morse code script incase you are in an immergancy. Maybe be chased by the disapproving gorilla at the Kalihari. The morse code script will blink ...---... or short short short long long long short short short repeat.

## Morse Code Challenge

Using either the Python interactive shell or a script, use the Gpiozero library and documentation at https://gpiozero.readthedocs.io/en/stable/api_output.html to create a morse code. When you are complete, check your anwser below. If you are impatient, you can just continue to the anwser.


## Morse Code Anwser

1. On the Raspberry Pi command-line open a new morse.py file using the nano text editor.
```
nano morse.py
```
2. Add the following Python code.
```
#!/usr/bin/env python3

import time
from gpiozero import LED

led = LED(21)
while True:
        led.blink(.5,.5,3, False)
        led.blink(1,.5,3, False)
        led.blink(.5,.5,3, False)
        time.sleep(5)
```
3. Exit nano using Ctrl+X.
4. Make script executable.
```
chmod 744 morse.py
```
5. Execute script.
```
./morse.py
```
6. End script with Ctrl+C.