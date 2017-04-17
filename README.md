# nodemcu-tm1638
Lua library for tm1638 (nodemcu, esp8266)

**First:**
This is a fork of a fork of csolg/nodemcu-tm1638

If i do something wrong with master and branch and pull-request etc... _SORRY!_ 
This is the first time i do that an i will read the GIT-Doc's asap to it better next time... ;-)

# What did i change:
I added the following Functions

## function module.setChar(address, char, dot)
- mask the address with 0x0F and make sure that all char are UPPER
 => call sendChar()
Thx to "cverbiest", his way to check a char is in font[] was much simpler then my way.

## function module.setLED(address, value)
- set the LED at address 0..7

## function module.test_modul()
- check every LED on the board

# Next to do:
- add getKey()

