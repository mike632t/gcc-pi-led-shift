## gcc-pi-led-shift

Written in C. 

Demonstrates how to write data to the GPIO pins of a MCP23017 I2C I/O port
expander.

Enables a single bit on the selected port of the I/O port expander and 
shifts it to the left and right alternatly a predefined number of times.  The
output can be used to drive an LED via a suitable current limiting resistor.

Note: You should NOT modify this code to enable more than two or three 
outputs at the same when driving LEDs directly from the MCP23017 as the total
output current for could easily exceed the maximum current rating for the 
device.  If you want to drive multiple LEDs at the same time you need to use 
a display driver or a transistor to switch the current.

