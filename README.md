# CP-01
Creality CP-01 profiles

I went through the factory gcode file and tried to create a custom cura profile for the CP-01 that fixes the 1st layer failure issue. 
These seem to work for me, but i'm sure they could be better. 

Let me know if you make a better one. 


Start Gcode

G90
M82
M106 S0
M140 S50
M190 S50
M104 S195 T0
M109 S195 T0
G28 ; home all axes
G92 E0
G1 E-10.0000 F4800
G1 Z0.335 F1002

End Gcode

G28 X0 Y0
M104 S0 ; turn off extruder
M140 S0 ; turn off bed
M84 ; disable motors
