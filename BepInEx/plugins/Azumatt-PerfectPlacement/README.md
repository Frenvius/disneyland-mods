# Description

### This mod is a variant of the following features from ValheimPlus and the author of the mod is not affiliated with the ValheimPlus team. This mod was created to be used by those that feel the existing replacements for these features are not good enough.

### The features are almost a direct pull from ValheimPlus and thus will stick to any updates that are made to the original features. If improvements can be made to provide compatibility with other mods, I will do my best to make them.

## FreePlacementRotation, AdvancedBuildingMode, and AdvancedEditingMode from ValheimPlus. This mod is a variant of these features from the mod and is not affiliated with the ValheimPlus team.

`Version checks with itself. If installed on the server, it will kick clients who do not have it installed.`

`This mod uses ServerSync, if installed on the server and all clients, it will sync all configs to client with the tag of [Synced With Server]`

`This mod uses a file watcher. If the configuration file is not changed with BepInEx Configuration manager, but changed in the file directly on the server, upon file save, it will sync the changes to all clients.`

## Source code for this variation can be found [here](https://github.com/AzumattDev/PerfectPlacement)

<details><summary>Configuration Options</summary>

`1 - General`

Lock Configuration [Synced with Server]
* If on, the configuration is locked and can be changed by server admins only.
    * Default Value: On

Enable Free Placement Rotation [Synced with Server]
* If on, Free Placement Rotation is enabled. Everything in section 2 will be affected.
    * Default Value: Off

Enable Advanced Building Mode [Synced with Server]
* If on, Advanced Building Mode is enabled. Everything in section 3 will be affected.
    * Default Value: Off

Enable Advanced Editing Mode [Synced with Server]
* If on, Advanced Editing Mode is enabled. Everything in section 4 will be affected.
    * Default Value: Off

Enable Grid Alignment [Synced with Server]
* If off, Grid Alignment is disabled overall, all code for it will be skipped. Everything in section 5 will be affected.
    * Default Value: Off

`2 - Free Placement Rotation`

Rotate Y [Not Synced with Server]
* The key to rotate the object you are placing on the Y axis, Rotates placement marker by 1 degree with keep ability to attach to nearly pieces.
    * Default Value: LeftAlt

Rotate X [Not Synced with Server]
* The key to rotate the object you are placing on the X axis, Rotates placement marker by 1 degree with keep ability to attach to nearly pieces.
    * Default Value: C

Rotate Z [Not Synced with Server]
* The key to rotate the object you are placing on the Z axis, Rotates placement marker by 1 degree with keep ability to attach to nearly pieces.
    * Default Value: V

Copy Rotation Parallel [Not Synced with Server]
* Copy rotation of placement marker from target piece in front of you.
    * Default Value: F

Copy Rotation Perpendicular [Not Synced with Server]
* Set rotation to be perpendicular to piece in front of you.
    * Default Value: G

`3 - Advanced Building Mode`

Enter Advanced Building Mode [Not Synced with Server]
* The key to enter Advanced Building Mode when building
    * Default Value: F1

Exit Advanced Building Mode [Not Synced with Server]
* The key to exit Advanced Building Mode when building
    * Default Value: F3

Copy Object Rotation [Not Synced with Server]
* Copy the object rotation of the currently selected object in ABM
    * Default Value: Keypad7

Paste Object Rotation [Not Synced with Server]
* Apply the copied object rotation to the currently selected object in ABM
    * Default Value: Keypad8

Increase Scroll Speed [Not Synced with Server]
* Increases the amount an object rotates and moves. Holding Shift will increase in increments of 10 instead of 1.
    * Default Value: KeypadPlus

Decrease Scroll Speed [Not Synced with Server]
* Decreases the amount an object rotates and moves. Holding Shift will decrease in increments of 10 instead of 1.
    * Default Value: KeypadMinus

`4 - Advanced Editing Mode`

Enter Advanced Editing Mode [Not Synced with Server]
* The key to enter Advanced Editing Mode
    * Default Value: Keypad0

Reset Advanced Editing Mode [Not Synced with Server]
* The key to reset the object to its original position and rotation
    * Default Value: F7

Abort and Exit Advanced Editing Mode [Not Synced with Server]
* The key to abort and exit Advanced Editing Mode and reset the object
    * Default Value: F8

Confirm Placement of Advanced Editing Mode [Not Synced with Server]
* The key to confirm the placement of the object and place it
    * Default Value: KeypadEnter

Copy Object Rotation [Not Synced with Server]
* The key to copy the object rotation of the currently selected object in AEM
    * Default Value: Keypad7

Paste Object Rotation [Not Synced with Server]
* The key to apply the copied object rotation to the currently selected object in AEM
    * Default Value: Keypad8

Increase Scroll Speed [Not Synced with Server]
* The key to increase the scroll speed. Increases the amount an object rotates and moves. Holding Shift will increase in increments of 10 instead of 1.
    * Default Value: KeypadPlus

Decrease Scroll Speed [Not Synced with Server]
* The key to decrease the scroll speed. Decreases the amount an object rotates and moves. Holding Shift will increase in increments of 10 instead of 1.
    * Default Value: KeypadMinus

`5 - Grid Alignment`

Align to Grid [Not Synced with Server]
* The key to enable grid alignment while building
    * Default Value: LeftAlt

Align Toggle [Not Synced with Server]
* The key to toggle grid alignment while building
    * Default Value: F7

Change Default Alignment [Not Synced with Server]
* The key to change the default alignment
    * Default Value: F6

</details>







<details><summary>How to Use/Additional Information</summary>

### Free Rotation Mode for the default Building Mode
* **Video demo: https://imgur.com/xMH7STj.mp4**
* This modifies the default build mode. How it works (all mentioned hotkeys can be modified):
    * Players can rotate the object selected in any direction while in the usual building mode by pressing certain hotkeys. The location of the object can be manipulated with the mouse:
        * ScrollWheel + LeftAlt to rotate by 1 degree on the Y-axis.
        * ScrollWheel + C to rotate by 1 degree on the X-axis.
        * ScrollWheel + V to rotate by 1 degree on the Z-axis.
    * Use the copy rotation hotkeys to copy the current rotation or apply the same rotation to the next object that is being built.
    * Build the object by clicking.

### Advanced Building Mode
* **Video demo: https://i.imgur.com/ddQCzPy.mp4**
* How it works (all mentioned hotkeys can be modified):
    * Players can freeze the item by pressing the configured key (F1 by default).
    * Players can modify the item position and rotation with the following key combinations:
        * Arrow Up/Down/Left/Right to move the building object in the respective direction.
        * Arrow Up/Down + Control to move the building object up and down.
        * ScrollWheel to rotate the building object on the Y-axis.
        * ScrollWheel + Control to rotate the building object on the X-axis.
        * ScrollWheel + left Alt to rotate the building object on the Z-axis.
        * Numpad plus/minus to either increase or decrease speed, holding SHIFT to raise/lower by 10 instead of 1 (Pressing Shift at any moment in time increases the distance/rotation angle 3 times)
    * Build the object by clicking.

**NOTE:**
* *Objects built with this system are not exempt from the structure/support system. Dungeons and other no-build areas are still restricted.*

### Advanced Editing Mode
* **Video demo: https://imgur.com/DMb4ZUv.mp4**
* You cannot be in Build mode (hammer, hoe or terrain tool). How it works:
    * Players can select the item with the configured key (Numpad0 is default).
    * Players can modify the item position and rotation with the following key combinations:
        * Arrow Up/Down/Left/Right to move the building object in the respective direction.
        * Arrow Up/Down + Control to move the building object up and down.
        * ScrollWheel = rotates the building object on the Y-axis.
        * ScrollWheel + Control to rotate the building object on the X-axis.
        * ScrollWheel + left Alt to rotate the building object on the Z-axis.
        * resetAdvancedEditingMode HotKey resets the position and rotation to the initial values.
        * Numpad plus/minus to either increase or decrease speed, holding SHIFT to raise/lower by 10 instead of 1 (Pressing Shift at any moment in time increases the distance/rotation angle 3 times)
    * Press the confirmPlacementOfAdvancedEditingMode Hotkey to confirm the changes. (press abortAndExitAdvancedEditingMode HotKey to abort editing mode and reset the object).

**NOTE:**
* *Other players will not be able to see the item being moved until the player building the item confirms the placement. Dungeons and other no-build areas are still restricted.*


### Grid alignment
* When pressing the configured key (left alt is the default) new buildings will be aligned to a global grid.
  The mode can also be toggled by pressing another key (F7 by default).
  Building elements (from the third tab) are aligned to to their size (e.g. a wood wall will have an alignment of 2m in X and Y direction). The alignment of building elements in other direction can be configured (by default with the F6 key) to 0.5m, 1m, 2m or 4m.
  Other buildings like furniture will always be aligned to 0.5m, but the Y position will not be aligned (to make sure they are always exactly on the floor).


</details>







<details><summary>
V+ Developer Credits

</summary>

# ValheimPlus Official Development Team [![ValheimPlus Icon](https://raw.githubusercontent.com/nxPublic/ValheimPlus/master/ico.png)](https://discord.valheim.plus)

* Kevin 'nx#8830' J.- https://github.com/nxPublic
* Miguel 'Mixone' T. - https://github.com/Mixone-FinallyHere
* Lilian 'healiha' C. - https://github.com/healiha
* Nathan 'NCJ' J. - https://github.com/ncjsvr

# Credits
* Greg 'Zedle' G. - https://github.com/zedle
* Paige 'radmint' N. - https://github.com/radmint
* Chris 'Xenofell' S. - https://github.com/cstamford
* TheTerrasque - https://github.com/TheTerrasque
* Bruno Vasconcelos - https://github.com/Drakeny
* GaelicGamer - https://github.com/GaelicGamer
* Doudou 'xiaodoudou' - https://github.com/xiaodoudou
* MrPurple6411#0415 - BepInEx Valheim version, AssemblyPublicizer
* Mehdi 'AccretionCD' E. - https://github.com/AccretionCD
* Zogniton - https://github.com/Zogniton - Inventory Overhaul initial creator
* Jules - https://github.com/sirskunkalot
* Lilian Cahuzac - https://github.com/healiha
* Thomas 'Aeluwas#2855' B. - https://github.com/exscape
* Nick 'baconparticles' P. - https://github.com/baconparticles
* An 'Hachidan' N. - https://github.com/ahnguyen09
* Abra - https://github.com/Abrackadabra
* Increddibelly - https://github.com/increddibelly
* Radvo - https://github.com/Radvo

</details>




<details><summary>Author Information</summary>

`Feel free to reach out to me on discord if you need manual download assistance.`

## My Information


### Azumatt

`DISCORD:` Azumatt#2625

`STEAM:` https://steamcommunity.com/id/azumatt/

For Questions or Comments, find me in the Odin Plus Team Discord or in mine:

[![https://i.imgur.com/XXP6HCU.png](https://i.imgur.com/XXP6HCU.png)](https://discord.gg/Pb6bVMnFb2)
<a href="https://discord.gg/pdHgy6Bsng"><img src="https://i.imgur.com/Xlcbmm9.png" href="https://discord.gg/pdHgy6Bsng" width="175" height="175"></a>
***

</details>