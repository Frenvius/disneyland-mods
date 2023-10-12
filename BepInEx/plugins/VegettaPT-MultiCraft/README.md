# MultiCraft
This is a simple mod that will add some UI elements that will let the user create multiple items with one click!

## Manual Installation
To install this mod, you need to have BepInEx. After installing BepInEx, extract CraftingStationLevelRange.dll into games install **"\Valheim\BepInEx\plugins"**

## About this mod.
This mod is a creation of Maximiliano Degue. The mods are being published under [MaxiMods Team in Thunderstore](https://valheim.thunderstore.io/package/MaxiMods/) and [mjdegue in Nexus Mods](https://www.nexusmods.com/valheim/users/89207773). This is the same person (myself).
If you need to report a bug, please, do it in the [MultiCraft NexusMods' section](https://www.nexusmods.com/valheim/mods/263?tab=bugs).
Thanks in advance!

## ChangeLog

### Version 1.2.0
* Added support to latest valheim update

### Version 1.1.1
* Added Mistlands support.

### Version 1.0.0
* Added Heart and Home support.

### Version 0.2.7
* Fixed issue where the MultiCraft UI would dissapear if logging off from the game.

### Version 0.2.6
* Fixed issue where when teleporting there was no MultiCraft UI anymore!

### Version 0.2.4
* Fixed issue where some recipes would show a wrong amount of items when upgrading.
* Reduce the verbosity in the logs.

### Version 0.2.3
* Pontential fix for a nullpointer reference that would break the functionality of MultiCraft

### Version 0.2.2
* Fixed a game-breaking bug where not having Craft from Containers plugin

### Version 0.2.1
* Now usable with "Craft from Containers" plugin!

### Version 0.2.0
* Adding extra controls for quicker updating crafting values
* Calculating maximum amount of craftable items based on items held by the user.
* Updating required items based on amount of items that will be crafted
* Adding amount of items held by the player for the required items (capped to 99)
* Fixed general bugs

### Version 0.1
* Add UI to craft Multiple Items
* Hijack the Crafting UI to hook MultiCraft systems on
* Loop Crafts to craft as many as the user wants
* Make sure no craftings are done if requirements aren't met
* Remove the posibility of MultiCraft in the Upgrade tab

## Backlog
* Adding config var that will allow users to not cap the limit the current possible maximum so they can use creative mod tools to craft x amount of things.