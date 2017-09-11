## Install stand offs for the Sense HAT

This is where we're going to deviate from what's inside the Astro Pi flight unit. The flight units have another circuit board in between the Raspberry Pi and Sense HAT which holds a real-time clock, an oscillator crystal, and a backup battery. This RTC board also has some pins that the six push-buttons connect to. Unfortunately, this is not available to the public.

Our goal was to keep the 3D-printed flight case as faithful to the original as possible, so the decision was taken to not alter it to accommodate the absence of this board. It may be possible for us to release the Gerber files for it in the future so that people can make their own. We're going to use hex nuts of the same depth as the RTC board to compensate for its absence.

+ Add the extended 23-way pin header to the Raspberry Pi GPIO pins, at the furthest end from the USB ports.

+ Then, take an 8mm M2.5 stand off and put a hex nut onto its thread before screwing it into the hole of the 11mm stand off, as shown below. Do the same for the remaining three stand offs.

![Add standoffs](images/add-header-standoffs.png)

WARNING|&nbsp;
---|---
![WiFi antenna](images/pi3_wifi.jpg)|A note for Pi 3 users. Using a **metal** stand off next to the wireless antenna will degrade its performance and range. The advice is to either omit this stand off from your build or to use a nylon stand off and nylon screw instead.

+ Do not install the Sense HAT yet as it will get in the way when you connect the GPIO pins to the buttons.
