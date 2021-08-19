# LmFaO
## LED LFO
This module is intended to drive LEDs with a simple but powerful LFO. The LEDs can be used with LDRs to control anything that you would normally control with a potentiometer/variable resistor. 

Because you can select an LDR value that suits your project, this module can be used to apply an LFO to virtually anything.

The module has adjustable Rate, Depth, and 4 possible waveforms to select from.

## Notes
* Designed and tested with 5v, but theoretically should work with up to 5
* Capacitor Value determines the range of speeds
  * Recommend a value between 10uF and 100uF
* Resistor R5 determines the max speed in the range
  * Recommend a lower value for Higher value capacitors
  * 220R for 100uF, 470R for 47uF, and 1k for 10-22uF all worked nicely in testing 
* Diodes only needed if you want to use the Saw Waveforms
* The Depth potentiometer just changes brightness and can be jumpered off/replaced with a set value resistor if adjustable depth is not needed for your application.
* Jumper switch connections if you only want 1 waveform
* Sample connections for 4 Way Selector switch (need 2 Pole 4 Position switch):
  * Square: P1C>P1Sq
  * Triangle: P1C>P1Tri
  * Saw: P1C>P1Tri, P2C>P2S 
  * Reverse Saw: P1C>P1Tri, P2C>P2RS 

## Parts List
* TL072 IC
* 100k Linear Pot for Rate Control
* 50k Linear Pot for Depth Control (optional, see Notes)
* 100uF Electrolytic Capacitor (default, see Notes on values)
* 1N4148 Diodes x2 (only needed for Saw Waves)
* Resistors:
  * 100k x2
  * 47k
  * 22k
  * 220R (default, see Notes on values)
* Incidental Parts (will vary by application)
  * Switches:
    * 2 Position, 3 Pin On/On Switch (for switchable Square/Triangle)
    * 3 Position, 3 Pin On/Off/On Switch (for switchable Saw/Triangle/Reverse Saw)
    * 4 Position, 2 Pole (10 Pin) Switch (for a single switch to select any of the 4 possible waveforms) 
    * A simple On/Off switch can be installed between the Voltage Source and the V+ input to turn the LFO On/Off
  * LEDs
    * Number will vary by project, schematic shows 5 in use but alter to suit your project
    * LED Resistors will vary depending on Voltage and LED color. Green LEDs worked very well with 5v and 220R Resistors

#### Donate with Sponsor Button Text 
