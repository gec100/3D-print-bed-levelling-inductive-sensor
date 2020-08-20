#With LJ18A3-8-Z/BX sensor#

![Image](https://www.diyelectronics.co.za/store/6088-thickbox_default/inductive-sensor-probe-lj18a3-8-zbx.jpg)

Had this sensor for long time working great on my custom made prusa clone and now I'm building a new corexy printer around SKR 1.4 Turbo board on 24V.

I'm not a electronics engineer but I can find my way around.

The sensor needs 6-36V to work properly, but probe connectors on the board can accept only 3-5V. On 12V boards this sensor needed to be connected to the 12V pin (spare Fan connector) with voltage divider described here http://reprap.com/wiki/Z_probe

In this 24V setup, resistors had to be changed. With https://www.allaboutcircuits.com/tools/voltage-divider-calculator/
I calculated that my resistors need to be roughly 4:1 (R1:R2) in size to get the output voltage below 5V needed for the Z-stop probe pins. That would be cca 4kΩ for R1 and 1kΩ for R2 or 8kΩ for R1 and 2kΩ for R2 . You get the point. I had at my hands 5k1 for R1 and 1k for R2 giving me cca 3.9V that is well inside 3-5V range.

here is my very rough schematics:

![Image](https://user-images.githubusercontent.com/8178773/89330570-be9fcd80-d690-11ea-98d7-8f2fd71f060a.png)
