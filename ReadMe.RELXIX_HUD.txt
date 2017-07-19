Red Eagle LXIX's Custom HUD : A16(b138) : v0.18

To use in Multi-player, the files need to be installed on the server/host of the game.

-----
INSTALL INSTRUCTIONS:
 1. Extract the contents of this zip into your 7 Days To Die Config folder 
    Default path is 
    "C:\Program Files (x86)\Steam\SteamApps\common\7 Days To Die\Data\Config"
 2. You should be prompted to replace SteamApps\common\7 Days To Die\Data\Config\xui.xml - say yes (if not, manually extract the file and overwrite)
 3. You should be prompted to replace SteamApps\common\7 Days To Die\Data\Config\XUi\windows.xml - say yes (if not, manually extract the file and overwrite)
 4. You should be prompted to replace SteamApps\common\7 Days To Die\Data\Config\XUi\controls.xml - say yes (if not, manually extract the file and overwrite)
 5. You should be prompted to replace SteamApps\common\7 Days To Die\Data\Config\XUi\styles.xml - say yes (if not, manually extract the file and overwrite)
 7. You should be prompted to replace SteamApps\common\7 Days To Die\Data\Config\XUI_Menu\xui.xml - say yes (if not, manually extract the file and overwrite)
 8. You should be prompted to replace SteamApps\common\7 Days To Die\Data\Config\XUI_Menu\windows.xml - say yes (if not, manually extract the file and overwrite)
 9. You should be prompted to replace SteamApps\common\7 Days To Die\Data\Config\XUI_Menu\controls.xml - say yes (if not, manually extract the file and overwrite)
 10. You should be prompted to replace SteamApps\common\7 Days To Die\Data\Config\XUI_Menu\styles.xml - say yes (if not, manually extract the file and overwrite)
    NOTE: say NO for styles.xml if you plan to use 7DTD Default Compass.  Either way this file is optional.

-----
UNINSTALL INSTRUCTIONS
 1. Verify Integrity of Game Cache in Steam client.

-----
Tweaking Instructions:

	Adjust UI size (FILE = xui.xml (Config\xui.xml && Config\XUI_Menu\xui.xml):
    1. Get a good text editor (not notepad).
    2. Open xui.xml
    3. Search for "<ruleset name="default" scale="1.255" stackpanel_scale="1.05">" without quotes (this is the default)
    4. Change the scale and/or stackpanel_scale to your preference.  Stackpanels are the floater notifications.
    5. Save the file.

	Basic removing of added windows (FILE = Config\xui.xml && Config\XUI_Menu\xui.xml):
    1. Get a good text editor (not notepad).
    2. Open xui.xml
    3. Search for "Delete this line to remove these items -->" without quotes.
    4. Find the line with the description that matches what you want to remove (example: "Window that displays Numbers on the tool belt for each slot").
    5. Delete the entire line.
    6. Save the file.

  Restoring the 7DTD Default Compass and Date/Time (FILE = Config\xui.xml):
    1. Get a good text editor (not notepad).
    2. Open xui.xml
    3. Search for "windowCompassRELXIX" without quotes.
    4. Replace "windowCompassRELXIX" with "windowCompass".
    5. RECOMMENDED To delete the "mapStatsHUD" and "mapCoordsHUD" lines right below (and labelled as such) when using default compass
    6. You do NOT need styles.xml if using the default compass.  If you do use it, the compass will still end up a bit wider.

	Adding disabled coordinates window windows (FILE = Config\xui.xml) (see NOTES below why this is disabeld by default):
	As of Alpha 16 this choice is not functional at all.  Enabling this now will cause Stack Overflow which will either crash 7DTD completely and/or cause other issues and bugs.

-----
Added:
Fixed: 
Changed:
 Updated for Alpha 16
Removed:

-----
Notes:
mapArea controller based window has been disabeld as of v0.09 due to a NRE when using waypoints
See the following posts for bug report and discussion on the issue:
  https://7daystodie.com/forums/showthread.php?39731-mapArea-Controller-not-respecting-XUI-for-Waypoint-amp-Click-Layer-Moving-map-window

As of Alpha 15b105 this is still an issue and why I leave this functionality disabled by default.  I believe mod authors have a responsibility to do no harm.
Moreso, if one knows a bug is a direct result of the functionality of a mod, an author of said mod has a DUTY to both the users of that mod and to the
developer of the game to inform uses of that mod of such potential issue.  Both so the user is aware they may have the issue, and so they know it is a bug
as a direct result of using said mod instead of reporting it as a game issue.

As of Alpha 16 this option cannot be enabled due to a Stack Overflow error that occurs which potentially can completely crash 7DTD or cause other errors and bugs.
I have not yet tried debugging this error using the new debug commands.
	As of Alpha 16 this choice is not functional at all.  Enabling this now will cause Stack Overflow which will either crash 7DTD completely and/or cause other issues and bugs.
	I have not yet tried debugging this error using the new debug commands.
    1. Get a good text editor (not notepad).
    2. Open xui.xml
    3. Search for "<!--<window name="mapCoordsHUD" />-->" without quotes.
    4. Replace with "<window name="mapCoordsHUD" />"
    5. Save the file.

-----
RANT TIME:
	I've noticed some mod authors have included/enabled some functions in recent mods by default.  
	Further claiming those mods to not be affected by reported/known bugs.
	Even after having been informed of being impacted by such bugs they've not informed their users.
	To me that is a disservice to both the users of said mod and to The Fun Pimps.
	Please note: This is my own personal opinion and rant.

-----
Reminder:
All changes in the XML files are tagged at the start and end of all changes with "Red Eagle LXIX's Custom HUD"

-----
Credit to The Fun Pimps for 7 Days To Die
Credit to Sirillion's HUD mod for early inspiration: http://steamcommunity.com/app/251570/discussions/5/494631967664775812
-----
-----
Thanks For the bug reports.  :)
-----
-----
-----
Thanks to The Fun Pimps for a good game.
-----
--
