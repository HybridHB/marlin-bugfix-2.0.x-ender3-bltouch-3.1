# marlin-bugfix-2.0.x-ender3-bltouch-3.1
These are the Marlin 2.0.x changes that works for my ender 3 pro with 1.1.4 board and official (Antclabs) bltouch 3.1 using the creatlity bltouch bracket. My ender 3 pro did not require removal of any capacitors.

Important!
In Configureation.h, change the following for your printer

X_PROBE_OFFSET_FROM_EXTRUDER
Y_PROBE_OFFSET_FROM_EXTRUDER
Z_PROBE_OFFSET_FROM_EXTRUDER

Z_PROBE_OFFSET_FROM_EXTRUDER is set to 0. If you know the z offset for your machine set it here.  If you dont it is ok to use 0, but you will have to find the proper z value for your machine, then store it to the eprom.

ABL is set to probe a 5x5 grid with extrapolation enabled, if you want to change the grid size update
GRID_MAX_POINTS_X

If you want to disable extrapolation, comment out
#define EXTRAPOLATE_BEYOND_GRID