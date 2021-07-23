Neptune 2 BL Touch Installtion:

DISCLAIMER: We recommend you reconfigure YOUR Config file and not use this provided file!  Instructions on how to Reconfigure your own file are available on the YouTube video and Blog post, both linked below. We are NOT RESPONSIBLE for any damage or issues using this file or instructions may cause, USE AT YOUR OWN RISK!

Config file provided (Config File - READ README FIRST.txt) is for installation of the ANTCLABS BL Touch on the Elegoo Neptune 2 ONLY.

- If you choose to use the pre-configured file, just rename it to "elegoo.txt" and place that on your SD card.  Insert SD Card into an OFF Neptune 2, then turn it on.  Done.

Requires BL Touch Mount (provided Config is for this SPECIFIC mount.):

---------------------------------------------------------------------------------------------------------------------------------------

File install Procedure:
1) Rename the Config file to "elegoo.txt" and place the file on your Printer's SD Card.  
2) Power Off the Printer
3) Insert the SD Card
4) Turn on the Printer
5) Perform Z-Offset Procedure to configure sensor to specific machine.

Detailed Installation Instructions:
- How-To YouTube Video: https://youtu.be/7jILw_2lRDw
- How-To Blog Post: https://www.hotrodhippie.com/post/bl-touch-install-on-elegoo-neptune-2-how-to

-----------------------------------------------------------------------------------------------------------

Configuration information to configure your own "elegoo.txt" file:

- Download latest Config file from Elegoo.com: https://www.elegoo.com/pages/3d-printing-user-support

- We recommend using Vistual Studio Code or Notepad++ to edit this config file, NOT your standard Notepad app.


Neptune 2 “Elegoo.txt” Config File Changes for BL-Touch:
------------------------------------------------------------------------------------------------------------

============ Bed Leveling ============

>cfg_leveling_mode  0 or 1   (This does NOT Enable Auto-Bed leveling.  This just chooses which menu shows up on "Tool" menu "Manual Leveling" or "Auto-Leveling".  I recommend leaving this as 0, as that will retain the Manual Bed Leveling option.  You can change this to 1 and it will present a "Auto-Leveling" option but that takes away the Manual Leveling setup, thus making later Manual Leveling more difficult.  Auto Bed Leveling is NOT a replacement for Manual Leveling, you will still need to manual level occassionally.)

============ Auto Leveling ============

No changes necessary here, but take note of these commands for your Slicer “Start G-Code” we will change later.

============ Endstop Settings ============

>USE_ZMAX_PLUG  2    (Default is 0, change to 1)

============ Z Probe Options ============

#BLTOUCH   1   (Default is 0, change to 1)

>Z_MIN_PROBE_PIN_MODE  2     (Default is 0, change to 2)

NOTE: The next 3 settings are the location of the Sensor in relation to the Nozzle (verify by measuring yours). These numbers apply to using MY MOUNT ONLY.  I cannot provide these numbers if you are using another design or modify the design I provided, do so at your own risk. Double check these measurements by physically measuring for best results as print variation or mounting variation can occur.

>Z_PROBE_OFFSET_FROM_EXTRUDER	0		
>X_PROBE_OFFSET_FROM_EXTRUDER	50.279  (Default is 32.55, change to 50.279)	
>Y_PROBE_OFFSET_FROM_EXTRUDER	-4.048   (Default is -7, change to -4.048) 	

>Z_SAFE_HOMING   1    (Default is 0, change to 1)

============ Bed Leveling ============

>BED_LEVLING_METHOD   3   (Defualt is 0, Change to 3)

Optional: Change the below settings to probe more points across the bed.  This increases the time Bed Leveling will take, but provides more accurate results.

>GRID_MAX_POINTS_X 	3   (Default is 3, change to anything BELOW 15)
>GRID_MAX_POINTS_Y 	3   (Default is 3, change to anything BELOW 15)

>Z_CLEARANCE_DEPLOY_PROBE   10   (Default is 20, Change to 10. Height the probe lifts before deploying, 20mm is overkill and slows things down.)

>Z_CLEARANCE_BETWEEN_PROBES   10   (Default is 20, Change to 10. Height the probe lifts between test points, 20mm is overkill and slows things down.)

============ Z Probe Settings  ============

>BLTOUCH   1   (Default is 0, change to 1)

---------------------------------------------------------------------------------------------------------------


Detailed Installation Instructions:
- How-To YouTube Video: https://youtu.be/7jILw_2lRDw
- How-To Blog Post: https://www.hotrodhippie.com/post/bl-touch-install-on-elegoo-neptune-2-how-to


DISCLAIMER: We recommend you reconfigure YOUR Config file and not use this provided file!  Instructions on how to Reconfigure your own file are available on the YouTube video and Blog post, both linked below. We are NOT RESPONSIBLE for any damage or issues using this file or instructions may cause, USE AT YOUR OWN RISK!
