# Sovol_ZERO_custom_config
A modular set of .cfg files that replaces the stock config.cfg.  

Written from scratch, it replaces the poorly written Sovol macros and adds features like e.g. filament-dependent chamber, nozzle wipe and cooldown temperatures, a PID-controlled exhaust fan, a recirculating Filter, a more human-readable Mainsail-interface (e.g. correct fan namings) and makes parameter tuning simpler by using variables. 
In particular, START_PRINT is improved: the stock macro can produce an incorrect Z-offset because filament oozes after the nozzle wipe and before contact probing.  

Some macros (e.g., START_PRINT) require parameters parsed from the slicer. The required custom G-code for parsing these parameters is included in the corresponding .cfg file in the corresponding macros.  
If any parameter is missing or wrong, the print is cancelled. This way, the machine won't execute any gcode which is generated for another printer setup. 
