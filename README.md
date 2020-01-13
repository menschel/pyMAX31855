# max31855

This module is a Python3 based interface to a max31855 with k-type thermocouple.

It was tested on a raspberry pi 0 with (adafruit breakout board)[https://www.adafruit.com/product/269].

The python module adafruit did provide was apparently broken or not tested properly.

# usage example
This will print 
```
from pprint import pprint as pp
import time
from max31855 import max31855
obj_ = max31855(bus=0,device=0)
try:
    while True:
        pp(obj_.read_value())
        time.sleep(5)
except KeyboardInterrupt:
    pass
```
