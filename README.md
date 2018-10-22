# DS1302_CircuitPython
Quick and easy library for the DS1302 RTC on CircuitPython

*This project is a port of SourcePerl's rpi.rtc library*
[rpi.rtc](https://github.com/sourceperl/rpi.rtc)


### What is this?
Glad you asked! This is a simple support library for the DS1302 RTC module on CircuitPython. The code has been tested on various Adafruit SAMD21-based microcontroller boards. The library *should* work on ESP8266, but the internal RTC of the ESP8266 has a drift and overflow issue when it comes to timekeeping, which may or may not impact the reliability of this library on the platform.

### How do I use this thing?
Have a look at main.py. You'll want to import the ds1302 module as well as the rtc module. Then, define the clock, data and enable pins which you'll use to instantiate the ds1302 class.

### Why is this a "quick port"?
Well, I really didn't optimize anything for CircuitPython yet. Also, the EEPROM routines are currently not implemented. There may still be some Godzilla-like bugs in there, so do not use this library for your *supasecret and revolutionary atomic clock replacement project*.
