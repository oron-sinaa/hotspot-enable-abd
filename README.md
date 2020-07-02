# hotspot-enable-abd
This windows powershell srcipt turns on "mobile-data" & "wifi-hotspot" on execution on stock Android 9.0 at least (without touching the screen)

---------------
// Description:
---------------

1. Enables mobile-data
2. Opens "hotspot & tethering settings"
3. "keyevent 20" presses down key to reach Wifi hotspot tab
4. "keyevent 66" presses enter key on Wifi hotspot tab
5. "keyevent 66" toggles Wifi hotspot setting ON
6. rest keyevent are to go back and lock screen after enabling data and hotspot

----------------
// Instructions:
----------------

1. You need to have adb downloaded on your PC (Google to download, easily available under 8MB
2. You need to have developer options "enabled" on your android device (tap "build number" 5 times under "about phone" to enable it)
3. You need to enable USB Debugging under Developer Options 
4. Connect your phone using USB and select "File Transfer - MTP" on your phone
5. When asked for USB debugging permission, allow (and tick remember for further convenience)
6. Paste this script in the ABD folder
7. Right click on this file and click "Run with PowerShell"

-------------------
// Troubleshooting:
-------------------

- Make sure your phone screen is unlocked
- The settings/tabs on your phone might be in some different order. To correct this, just check the sequence you go on your phone and edit the script as per requirement
- Use the relevant keyevents for your edit:-
      19 -->  "KEYCODE_DPAD_UP" 
      20 -->  "KEYCODE_DPAD_DOWN" 
      21 -->  "KEYCODE_DPAD_LEFT" 
      22 -->  "KEYCODE_DPAD_RIGHT" 
      66 -->  "KEYCODE_ENTER" 
      4 -->  "KEYCODE_BACK"
      26 -->  "KEYCODE_POWER" 
      
Enjoy! And sorry if you could not use your touch-screen to enable debugging and all.
Just make sure your phone screen is unlocked.
