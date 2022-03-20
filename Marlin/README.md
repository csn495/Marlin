# BigTreeTech SKR E3 Turbo in Ender 5

This board is larger than the other SKR Mini E3 and Creality boards and interferes with the power supply in the Ender 5 electronics case.

I (lpla) did a simple adapter for the power supply that can use short M8 screws and bolts (glued to this adapter): https://www.thingiverse.com/thing:4676935

That way the PSU gives enough space for the board to be drop-in replace. So all components fit inside the electronics case and are hold properly.

Regarding wiring, electronics case fan should be connected to the FAN2 pins.

This folder contains configuration files for Ender 5 using v2.0.X Marlin.

To compile, just use these config files and set `default_envs = LPC1769` in platformio.ini file.



# Beginning of changes made by CSN495

3/19/2022:  

    Replaced stock Z-axis leadscrew with Reliabot 400mm T8 Tr8x2 lead screw (2mm Pitch, 1 Start, 2mm Lead) + POM anti backlash nut.
    
    Changed Default steps per mm from 800 to 1600 in Configuration.h (See below).
            
        DEFAULT_AXIS_STEPS_PER_UNIT   { 80, 80, 800, 93 }   >   DEFAULT_AXIS_STEPS_PER_UNIT   { 80, 80, 1600, 93 }