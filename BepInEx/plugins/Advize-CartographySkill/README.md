![](https://staticdelivery.nexusmods.com/mods/3667/images/394/394-1617094724-435479074.png)

| [Description](#description) | [Installing](#installing) | [Contact Author](#contact-author) | [Other Info](#config-and-other-info) | [Config](#config) | [Source](#source) | [Changelog](#changelog) | [Screenshots](#screenshots) |
|---|---|---|---|---|---|---|---|

## Description
Ever sailed past a visible coastline, but it didn't appear on your world map? That's because the default radius around the player that is uncovered on the world map is smaller than your view distance! This mod allows you to increase that explore radius over time as you uncover more of your map.

This mod also includes a craftable spyglass item that doubles as a weapon. Use it to bash your enemies or to see their cowardly faces up close... but from a safe distance! Uses custom mesh, textures, and logic.

The custom skill as well as the spyglass can be enabled/disabled via the mod's config file, generated after the mod is loaded at least once (see Config & Other Info below).

Crafted and upgraded at a workbench. By default, right click will zoom in. Hold left shift and press right click to decrease zoom level by 1. Optional third key can be set to fully zoom out, or press 'r' to sheathe your Spyglass. Controls and functionality are configurable.

Recipe is: 2x Obsidian, 2x Bronze, 1x Crystal

## Installing

### Manual Install

Extract the Advize_CartographySkill.dll file into your BepinEx/plugins folder.
Directory structure should look like this:
```
BepInEx ->
    plugins ->
        Advize_CartographySkill.dll
```
## Contact Author
You can reach me on the Nexus to provide bug reports or feedback https://www.nexusmods.com/valheim/mods/394

## Config and Other Info:
Mod is highly configurable, a config file will be generated after first loading the mod and can be found in ﻿BepInEx/config/advize.CartographySkill.cfg

Localization Support: A file named Advize_CartographySkill.json will be generated alongside the .dll file after the game is first launched. In it you will find the ability to change the Spyglass name and description text. Any changes made to this file will be loaded by the mod.

Note: As of 1.5.0: Clients will by default receive configuration settings from a server hosting the mod unless `ServerIsAuthoritative` is set to false in the config file (server side). However, settings falling under the [Controls] and [Troubleshooting] categories of the config file will not be enforced by the server. Though authoritative, servers will not permanently alter a client's locally stored configuration file.

This is thanks to a custom implementation of the AuthoritativeConfig code written by Nextek for their Speedy Paths mod.

This config can be edited out of game with a text editor, or modified in game using the Configuration Manager mod (recommended).
By default, one should be able to reach cartography level 100 before exploring an entire world; but it will not add xp for parts you've already discovered (yet). If you need to increase the level higher and you've discovered your whole world, you'll need to uncover parts of the map in a new world.

Controls can be changed in the mod config - use this as your guide: https://docs.unity3d.com/Manual/class-InputManager.html

Alternatively, take a look at the following list: https://gist.github.com/C0DEF52/b1168e6ed3d1f567fc919f2942037bab

~~If using mods such as Map Sync Mod to produce map discovery as a result of irregular means, use the custom console command 'cartxpsync' to allow cartography XP to be awarded for synchronized discoveries. At present, this must be entered manually after map data has been synced via another mod.~~

## Config
### Default Config File:
```
## Settings file was created by plugin CartographySkill v2.0.0
## Plugin GUID: advize.CartographySkill

[Controls]

## Key to increase zoom level. See https://docs.unity3d.com/Manual/class-InputManager.html
# Setting type: String
# Default value: mouse 1
IncreaseZoomKey = mouse 1

## Hold this key while pressing IncreaseZoomKey to decrease zoom level. See https://docs.unity3d.com/Manual/class-InputManager.html
# Setting type: String
# Default value: left shift
DecreaseZoomModifierKey = left shift

## Optional key to fully zoom out. See https://docs.unity3d.com/Manual/class-InputManager.html
# Setting type: String
# Default value: 
RemoveZoomKey = 

[General]

## Nexus mod ID for updates.
# Setting type: Int32
# Default value: 394
NexusID = 394

## Amount to increase base explore radius by per skill level
# Setting type: Single
# Default value: 1
RadiusIncreasePerLevel = 1

## BaseExploreRadius (Vanilla value is 100)
# Setting type: Single
# Default value: 100
BaseExploreRadius = 100

[Progression]

## Enables the cartography skill
# Setting type: Boolean
# Default value: true
EnableSkill = true

## Experience gain when cartography skill XP is awarded
# Setting type: Single
# Default value: 0.5
LevelingIncrement = 0.5

## Amount of map tiles that need to be discovered before XP is awarded (influences BetterUI xp gain spam)
# Setting type: Int32
# Default value: 100
TileDiscoveryRequirement = 100

[ServerAuthoritativeConfig]

## <Server Only> Forces Clients to use Server defined configs.
# Setting type: Boolean
# Default value: true
ServerIsAuthoritative = false

[Spyglass]

## Enables the spyglass item
# Setting type: Boolean
# Default value: true
EnableSpyglass = true

## Influences field of view when zoomed, recommended range is 0 (disabled) to 5
# Setting type: Single
# Default value: 5
FovReductionFactor = 5

## Increase/Decrease camera zoom distance
# Setting type: Single
# Default value: 5
ZoomMultiplier = 5

[Troubleshooting]

## Enable mod debug messages in console
# Setting type: Boolean
# Default value: false
EnableDebugMessages = false
```
## Source
Github Repo: [Advize_ValheimMods](https://github.com/AdvizeGH/Advize_ValheimMods)

## Changelog
### 2.0.1
- Added extra null reference error prevention.

### 2.0.0
- Updated for Hearth and Home.
- Removed SkillInjector dependency.
- Both cartography skill and spyglass item can now be enabled/disabled individually.
- Localization support added for spyglass name and description.

### 1.5.0
- Dropped MCE support in favor of AuthoritativeConfig.
- Embedded assets within .dll file.

### 1.4.0
- Changed skill hover description in skill window.
- Added MCE support for server admins.

### 1.3.7
- Consolidated Nexus and Thunderstore branches.

### 1.3.6
- Fixed README.

### 1.3.5
- Minor code cleanup.
- Added debug message.
- Packaged for Thunderstore.io release.

### 1.3.4
- Updated spyglass icon to match 3D model.
- Added fix for error when generating a fresh world.
- Changed debug messages to accommodate new code flow. Code refactoring.

### 1.3.3
- Fixed conflict with Valheim+ and potential conflicts with all other mods who adjust field of view.
	- From this day forward, when you are zooming in with the spyglass, YOU ZOOM IN WITH THE SPYGLASS.

### 1.3.2
- No more Better Archery conflicts, all spyglass zoom levels now work!
- Spyglass can be spawned via console using prefab name advize_item_spyglass.
- Fixed a fov calculation error.
- Added Nexus mod ID for update checks.
- Added debug messages for when debug messages are enabled.
- Console command 'cartxpsync' added for Map Sync Mod users.
- Other fixes.
	
### 1.3.1
- Correctly bumped mod version number.
	
### 1.3.0
- Replaced Spyglass model.
- Spyglass will no longer zoom in or out while the inventory is open.
	
### 1.2.0
- Added spyglass control options to mod config.
- Spyglass now renders during character select screen.
	
### 1.1.1
- Added spyglass related config settings.
	- Zoom distance and field of view reduction are now configurable.
	- Spyglass item can be disabled entirely.
	
### 1.1.0
- Added craftable Spyglass item with custom mesh, textures, and unique logic.
	
### 1.0.3
- Minor update. Final code cleanup before new (if any) features are added. No need to update if you have 1.0.2.

### 1.0.2
- Disabled debug messages by default, but added config setting to toggle.
	- This improves performance when traveling quickly or entering "exploremap" into the console.

### 1.0.1
- New icon.
- View radius will now decrease if skill level is lowered without having to reload world.
- Fortified logic to prevent unexpected behaviour.

### 1.0.0
- Created Mod.

## Screenshots

Skill in Skills Window

![](https://staticdelivery.nexusmods.com/mods/3667/images/394/394-1615440013-1118542910.png)

Spyglass 3D Model

![](https://staticdelivery.nexusmods.com/mods/3667/images/394/394-1616841778-336427634.png)

Spyglass Item Tooltip (Item icon is outdated)

![](https://staticdelivery.nexusmods.com/mods/3667/images/394/394-1616758430-1786122127.png)

No Zoom (Spyglass model in screenshot is outdated)

![](https://staticdelivery.nexusmods.com/mods/3667/images/394/394-1616064366-774143860.png)

1st Zoom Level

![](https://staticdelivery.nexusmods.com/mods/3667/images/394/394-1616064371-1211294329.png)

2nd Zoom Level

![](https://staticdelivery.nexusmods.com/mods/3667/images/394/394-1616064376-1529982099.png)

3rd Zoom Level

![](https://staticdelivery.nexusmods.com/mods/3667/images/394/394-1616064380-321218162.png)