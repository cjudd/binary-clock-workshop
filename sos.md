# SOS

This is a lab intended to test your ability to control LEDs and look up documentation. In this lab, you will create a SOS script incase you are in an emergancy. <!-- Maybe you are being chased by the disapproving gorilla at the Kalihari.--> The SOS script will blink ...---... or short short short long long long short short short repeat.

## SOS Challenge

Using either the Python interactive shell or a script, use the Gpiozero library and documentation at https://gpiozero.readthedocs.io/en/stable/api_output.html to create a SOS. When you are complete, check your anwser below. If you are impatient, you can just continue to the anwser.


## SOS Anwser

1. On the Raspberry Pi command-line open a new sos.py file using the nano text editor.

```
nano sos.py
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
chmod 744 sos.py
```

5. Execute script.

```
./sos.py
```

6. End script with Ctrl+C.

---

[NEXT](binary_clock.md)