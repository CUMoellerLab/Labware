# Laboratory Shaker

We needed an inexpensive and compact plate shaker for our anaerobic chamber. The [Crickit](https://www.printables.com/model/7244-crickit-lab-shaker) Lab Shaker, remixed by [DotScott1](https://www.thingiverse.com/thing:3142779), was the perfect inspiration!

![Shaker shaking](./Images/shaker.gif)

I modified the original Crickit project to use the same inexpensive electronics as DotScott1's remix, but with a few modifications to fit our needs. The case is changed from three parts to two, with the entire upper part of the case a single print, and with all of the electronics mounted to the top. The bottom case panel now includes places to press-fit neodymium magnets to help prevent the shaker from moving around, and can be screwed firmly into the top case with countersunk machine screws. There's now also a nifty printed 'volume' indicator for the PWM potentiometer. :)

To save space in the incubator, these are all powered off of an Amazon USB charger with right-angle USB connectors. I tested to ensure that the charger would supply up to the 1.2 A stall torque for the DC gearmotor.

Check the included Excel spreadsheet for order links and prices.


## Printing and assembly


All parts were printed without supports, except for the linkages. Note that you need two idler linkages per shaker!

Assembly is pretty straightforward, and mostly follows the instructions from the original Adafruit build. I used nuts, washers, and blue Loctite for all screws except the blind-end holes for mounting the base and the circuit board.

### Electronics assembly

Cut off all but about 2 inches of the cord from the panel mount USB connector. Remove all of the external rubber cable guard, the insulation, and the green and white wires. Strip a few mm of insulation from the red and black wires and connect them to the Power + and Power - terminals on the PWM board, respectively. Then connect the red and black wires from the DC gear motor to the Motor + and Motor - terminals on the board.

Solder the ceramic capacitor between the two motor leads, right next to the motor. This will limit the spike in current throught the motor windings on startup, helping to extend its lifetime.

Mount the USB connector to the enclosure shell with the included M3 screws. Pull the plastic knob off the PWM board, remove the nut, and push the metal potentiometer shaft through the corresponding hole in the enclosure. Tighten the nut back on to retain the potentiometer shaft in the housing. You can affix the board using short M3 screws.


