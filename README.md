# firmware
A place for OldMan2525 binary builds of various Voxelab Aquila Marlin firmware

In the manualmesh folder is my build of Alex_qm's Marlin UI extended firmware 1.2.2A for the Voxelab Aquila printer. Special things I've enabled:
4x4 bi-linear manual mesh
PIDTEMPBED with defaults appropriate for the Aquila (but please run "M303 E-1 C8 S65 U" to make the values more closely match your exact machine)
PIDTEMP nozzle defaults are from my Aquila for 205C, instead of some long forgotten Ender 3 V2. Run "M303 E0 C8 S205 U" to make values special for your machine.
S Curve Acceleration, which I find cuts down on vibration substantially.
Preheat menu item PLA changed to PLA+ 205C nozzle, 65C bed
Serial communications over the USB port has been restored to 115200 bps.
Possibly a few other insignificant things I'd have to check my notes for

This firmware assumes you have an STM32F103, rather than a Giga Devices chip. If it flashes fine, you are good to go. If not, you'll have to check to see if you have a GD32 processor.
