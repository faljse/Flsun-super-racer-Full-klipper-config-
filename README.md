# Flsun-super-racer-Full-klipper-config-NANO SKR 1.3 VERSION COMING SOON (yes this is for stock printers with out mods ) 
  This readme is currently under construction more info will be added over time.

Complete Kllipper based on klipper docs and flsun marlin. routinely updated with the same functionality and higher spec 
 This config is currently compatible with cura after minor klipper specific changes to start gcode under printer settings version 4.12. The 4.10 cura should work by default.
in cura the start gcode is setup to use relative extrusion. this must be enabled in the profile otherwise random movments can and will occure. make sure to change both stock   profiles. This config is setup like a tutorial island the settings must be enabled for it to work. This is to attempt to lessen the learning curve if you can compile marlin. and to ensure that individual machines are setup to their indivial values. every machine is a bit different due to qc and, assembly. 
 
 OTHER HARDWARE / REOMMENDED BUT OPTIONAL.
  HDMI Capacitive Lcd for KLIPPER SCREEN. This grants nearly full acess to a clean ui with most klipper settings / standard printer controls in a modern touch ui  
it should be noted the stock. lcd more then likely will not be added to Klipper by developers anytimee soon (months/years) theres many other more common screens 
stil waiting for support. This is mostly a manufacture issue / semi propriatary software and tfts running their own firmware. if you don't want to use a pc / cell phone don't    wait up. Notes on klipper screen this removes most of the need for fluidd / mainsail other then uploads. IT makes certain features easier such as setting up zoffset / baby stepping. It also has visual bed mesh , wifi selection , and, what you'd expect control wise from a graphical marlin screen in terms of settings / control. 
 
USEFUL LINKS AND RESOURCES / INFO TO BE BECOME FAMILIAR WITH
https://klipperscreen.readthedocs.io/en/latest/ FULL TOUCH UI FOR CAPACITIVE HDMI TFT OR RESSISTIVE. TFT I USED / STL https://www.thingiverse.com/thing:2798667
https://www.klipper3d.org/Installation.html The offical manual 
https://www.klipper3d.org/Rotation_Distance.html?h=extr Extruder calibration docs 
Manual input shaper https://www.klipper3d.org/Resonance_Compensation.html?h=input
https://docs.fluidd.xyz Fluid web ui a premade raspberry pi image with everything require is also here. 
https://docs.mainsail.xyz/update/klipper Main sail web ui (more current / active updates at this time. ) either ui / image is entirely a matter of preference. 
https://github.com/th33xitus/KIAUH Kiauh installer script useful to have to update or some times fix certain problems via reinstall 
https://www.balena.io/etcher/ belena etcher a tool used to either clone or install images to sdcard for the raspberry pi. this can be very useful for multiple printers. the sdcard can simply be cloned and, config changed 
https://winscp.net/eng/index.php a gui ssh client to edit files on the raspberry pi. 

 WHATS NEW 
Bed mesh works on this copy provided the probe is with in range 
Correct values for stealth chop. note their are only 2 options hybrid will loose torque and cause layer skips and excessive noise as seen on other configs. 
Pressure advance (klippers equivalent to linear advance ) 
Thermal runaway is enabled by default in klipper. the configs for it must be added to make changes. default internal values should be fine. if its triggering more then likely Wrong pid or somthing is loose on the hotend or bed. it will only go of if it has reason to. 
1/128 stepping 
High torque / tuned tmc drivers 
Fluidd or Mainsail web ui 

WHAT NOT TO DO 
 Once everything is installed, due to printers offsets being different it is suggested  to raise the z offset in fluidd or mainsail 1 or 2mm to then lower it incrimentally on a test print.This is a good safety measure  to ensure the measured value were correct. It is also recommended to test the probe via probing into a hand to ensure its working with the other hand on the power if it doesnt stop for whatever reason. 
 Do not enable listed features in slicer that are known to be incompatible. those can be found on the klipper slicer docs on the website listed. 
 Do not assume square corner velocity is the same as jerk its not the same. klipper runs on different motion software similar to junction deviation usually 5-7 on the sr is good and high acceelration. there are exceptions to this eg low accelleration  higher square corner for smaller prints with lower acceleration. 

GENERAL DISCLAIMER use at your own risk I am not responsible for any resulting damages or miss use. All setting are setup to be in spec to the orginal marlin 1.3 firmware or close due to firmware differences. The speed is however setup to be faster and resolution is 3x higher then  marlin on the steppers. In general it is a bit more quiet.

If you like the work and, want to buy me a coffee https://www.paypal.com/paypalme/danorder 


