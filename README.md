# Anet-A8-Marlin
Configs for my upgraded Anet A8 running a stock controller

I inherited an [Anet A8 variant from Alunar. It was an A8 3D printer](https://anet3d.com/pages/a8) and I made the following changes to the hardware.

1. Replaced the power supply. The old one was of quetionable quality.
2. Added a power switch with a fuse and cover for the PS terminals. The manufacturer had the user wire the plug into the powersupply. Really.
3. Added a MOSFET for the bad. The controller was sending real wattage to the bed. Now the controller sends a signal to the MOSFET and the MOSFET had it's own connection to the new powersupply.
4. I 3D printed a controller case, tensioners for the X and Y and braces for the bed. The acrylic frame is awful but the braces help keep it rigid.
5. Added a PEI covered spring steel magnetic bed.
6. Added a 12mm diameter 5V indcutive probe. That is wired into the Z endstop and works well.

I'm using the stock Anet A8 Marlin configs with very few chanegs.

1. Removed SD card support. The SD card is inside the printed case and I print via the USB port.
2. Enabled bed tramming in the LCD menu. This is one of my favorite Marlin built in options.
3. Enabled fixed bed probe and a 50mm margin. That's a lot but less than that and my X and Y carriages hit the frame.

I've copied the Cura Ender 3 start code except I moved the purge line in 3mm. I could fix X=0 in Marlin but this is easier.
