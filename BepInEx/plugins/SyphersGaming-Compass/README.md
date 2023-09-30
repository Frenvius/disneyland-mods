This mod adds a rotating compass to the HUD that shows nearby map markers.

You can customize:

The png file used to display the compass (there's a GIMP xcf file included that you can use as a template)
The png file use to mask the compass (determines how wide to display the compass)
The png file use to show the center marker (a line showing the center of the screen)
Whether to show the center marker
The color and transparency of the compass
The color and transparency of the center marker
The color and transparency of the map markers
The maximum distance to show map markers
The size of the compass
the offset from the top of the screen


Ignore Lists

In the config, there is a list of marker names to ignore and a list of marker types to ignore.

The default value for marker names to ignore is Silver,Obsidian,Copper,Tin which are the names of markers added by AutoMapPins. You can also use prefixes appended with an asterisk (*), e.g. Dungeon* for ignoring any marker staring with Dungeon.

The list of possible types to ignore is included in the config comment.


Config

A config file BepInEx/config/aedenthorn.Compass.cfg is created after running the game once with this mod).

You can adjust the config values by editing this file using a text editor or in-game using the Config Manager﻿.

To reload the config from the config file, type compass reset into the game's console (F5).


Technical

To install, place the zip file contents in the BepInEx/plugins folder. You will need BepInEx.

Code is at https://github.com/aedenthorn/ValheimMods.

﻿﻿If you want to complain or ask for help or help me test my mods, you can visit my Discord server﻿.

Click here for a list of all my mods for Valheim.
