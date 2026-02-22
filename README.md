# Sovol_ZERO_custom_config
A modular set of .cfg files that replaces the stock config.cfg.  
Written from scratch, it replaces the poorly written Sovol macros and adds features like e.g. filament-dependent chamber, nozzle wipe and cooldown temperatures, a PID-controlled exhaust fan, a more human-readable Mainsail-interface (e.g. correct fan namings) and makes parameter tuning simpler by using variables. 
In particular, START_PRINT is improved: the stock macro can produce an incorrect Z-offset because filament oozes after the nozzle wipe and before contact probing.
