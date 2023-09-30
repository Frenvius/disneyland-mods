![](https://staticdelivery.nexusmods.com/mods/3667/images/1042/1042-1618905952-462602285.png)

| [Description](#description) | [Features](#features) | [Installing](#installing) | [Compatibility](#compatibility) | [Contact Author](#contact-author) | [Other Info](#config-and-other-info) | [Config](#config) | [Source](#source) | [Screenshots](#screenshots) |
|---|---|---|---|---|---|---|---|---|

## New
Looking to make your farming life simpler and more efficient? Try my latest mod, [Plant Easily](https://valheim.thunderstore.io/package/Advize/PlantEasily/). It allows you to plant evenly spaced crops, either one at a time or in any amount of rows and columns, with grid snapping features and invalid crop placement prevention. It also allows bulk harvesting of resources and auto-replanting of crops. It's highly configurable and includes gamepad support. Most importantly, it supports vanilla crops, saplings, and the pickable resources added by Plant Everything.

## Description
A rewrite of the Planting Plus mod by bkeyes93. Plant Everything allows you to plant and harvest gathered and pickable resources found throughout the world, such as berry bushes, mushrooms, thistle, dandelion, as well as previously unavailable saplings and decorative flora. Expand your farming repertoire with berry bushes, flowers, and mushrooms whose resources will respawn over time. While you're at it, spruce up your settlement with some small trees, bushes, and even wall-mountable vines!

In addition to the added plantable resources, a wide range of configurable options allows you to tweak the mod/game's farming related aspects in favor of aesthetics, game balance, or your personal preference. By default the configuration file is centered around game balance and respects all of the vanilla game settings. This includes its obscenely long respawn time for pickables, which can range as high as several hours of real time spent in the game. I strongly encourage you to lower your pickable respawn times for a more enjoyable experience.

`If you need to remove a spawner, aim at it and press your deconstruct key (middle click by default) with your cultivator in your hand the way you would destroy a building piece with your hammer equipped.`

## Features

This mod adds a wide range of features, some of which are not well known (or even forgotten), but all of which are toggleable. I'll do my best to provide as comprehensive a list as I can, and will update it over time. The following is a short list of some of the most significant features.

**Adds 24 recipes to the cultivator**
- which are unlocked by obtaining at least 1 of each of the recipe's required materials, as you would any other recipe in the game.

**Provides the option to grow crops in any biome.**
- Also allows you to remove other restrictions such as whether crops need cultivated ground, open sky, space to grow, or even whether you can plant your trees indoors.

**Displays growth time remaining**
- on crops, pickables, and saplings as hover text. See [UI] section of config for related settings and toggling it on/off.

**Personalize numerous game settings**
- relating to crops, saplings, pickables, and seeds. These settings include growth times, costs, yields, grow radius, and size scaling.

**Remove pesky respawning debris**
- such as sticks, stones, and flint using your cultivator (see bold text at end of 'Description' section). Also allows you to set resource cost and return of debris.

**Plant some flora indoors.**
- When [Difficulty]PlaceAnywhere is enabled, the following changes take effect: Saplings, small trees, and bushes can be placed indoors. Saplings can grow into trees indoors, and sapling grow radius is ignored. Bushes and saplings/trees placed while PlaceAnywhere is enabled will defy gravity (to prevent them from falling through floors). Even if PlaceAnywhere is later disabled, the pieces will continue to float until the world is loaded without the mod present.

**Synchronizes configuration settings in multiplayer using ServerSync.**
- Mod configurations will be synchronized between connected clients who are using the mod. If [General] LockConfiguration is set to true, only server admins will be able to modify configuration settings. However, settings falling under the [General] category of the config file will not be synchronized (with the exception of EnableMiscFlora). Though ServerSync will sync configs between connected clients, a client's locally stored configuration file will not be altered.

**Supports localized text**
- for the added plantable resources. The mod does offer localization support, but the mod has yet to be translated to other languages. Users can help to translate the mod to other languages by enabling "EnableLocalization" in the config, and then re-launching the game once. This will generate a .json file in the plugins directory alongside Advize_PlantEverything.dll named 'english_PlantEverything.json'. Using any text editor, edit the names and descriptions in the right column and resave the file as '{language}_PlantEverything.json'. Finally, change the language setting in the mod's config file to match {language} of your json file. For example, if you launch the game while "spanish_PlantEverything.json" is present alongside the .dll file AND the config language option is set to "spanish", it will load strings for names and decriptions from the Spanish json file.

If you are willing to translate to other languages, I would be more than happy to offer them as optional downloads with the mod.

**Miscellaneous Features:**

- Custom meshes for flowers and mushrooms to indicate picked status. Picked models will not display on clients without the mod or who have ShowPickableSpawners set to false, but the spawner will remain and will display again once matured.
- Works in multiplayer environments even for users without the mod. Unmodded clients will be able to see and interact with all of the added resources that you plant. However, some settings may only work if the mod is installed on the server as well.
- Snap points can be seamlessly toggled on/off for vines to help with placement using Configuration Manager.
- Many pickable resources can be disabled by setting their resource cost to 0. Eligible resources will mention it in the description of their respective config settings.

The following recipes have been added to the cultivator:

Raspberry Bush, Blueberry Bush, Cloudberry Bush\
Mushrooms, Yellow Mushrooms, Blue Mushrooms\
Thistle, Dandelion\
Ancient Sapling, Ygga Sapling

With EnableMiscFlora enabled in config:

Small Beech Tree, Small Fir Tree, Small Dead Fir Tree\
Small Plains Bush, Small Fruitless Bush (2 tints), Small Shrub (2 tints)\
Vines, Glowing Mushroom\
Branch, Stone, Flint

## Installing

### Manual Install

Extract the Advize_PlantEverything.dll file into the BepInEx/plugins folder.
Directory structure should look like this:
```
BepInEx ->
    plugins ->
        Advize_PlantEverything.dll
```
#### In multiplayer environments:
It is strongly recommended you install the mod on the server, though it is not required for all settings and features. Other connected clients are encouraged to use the mod as well, but that too is not a requirement.
## Compatibility
Here you'll find info about known mod conflicts and possible solutions.

### Valheim+:
Though compatible out of the box, Valheim+ does have some config settings that can overlap with settings from Plant Everything. Only if and when these specific features are desired from one mod or the other will you have to decide which mod's feature you'd prefer to use. Doing so is as simple as toggling something on/off in either of the mod's config files.

### PlantEasily:
There are zero conflicts between this and PlantEasily, as it was designed to compliment this mod and vice versa.

### Farming:
While there can be overlap between config options, there are no hard conflicts with Farming by smoothbrain. I do recommend you study the config files for each mod and choose which mod will drive the features that best suit your needs.

### MassFarming:
There are no conflicts between this mod and MassFarming, but as far as I know it still does not support the pickable resources added by this mod (berry bushes, flowers, mushrooms).

### EasyFarm:
There are no conflicts between this mod and EasyFarm, but as far as I know it still does not support the pickable resources added by this mod (berry bushes, flowers, mushrooms).

### FarmGrid:
The FarmGrid config file requires a bit of tweaking in order to support the resources added in this mod. See following guide.
```
Open your FarmGrid config file in a text editor or in game using the Configuration Manager mod. Find the line beginning with

plantObjectMasks =

Change it to:

plantObjectMasks = piece, piece_nonsolid, item

Find the line beginning with

﻿customPlants = 

Change it to:

customPlants = RaspberryBush(Clone): 0.5, RaspberryBush: 0.5, BlueberryBush(Clone): 0.5, BlueberryBush: 0.5, Pickable_Mushroom(Clone): 0.5, Pickable_Mushroom: 0.5, Pickable_Mushroom_yellow(Clone): 0.5, Pickable_Mushroom_yellow: 0.5, Pickable_Mushroom_blue(Clone): 0.5, Pickable_Mushroom_blue: 0.5, CloudberryBush: 0.5, CloudberryBush(Clone): 0.5, Pickable_Thistle(Clone): 0.5, Pickable_Thistle: 0.5, Pickable_Dandelion(Clone): 0.5, Pickable_Dandelion: 0.5


Tweak grid spacing as you see fit. If spacing seems off to you, replace the traditional decimal format for spacing with the following:
0.15 = 15e-2
0.25 = 25e-2
0.5 = 5e-1
0.75 = 75e-2
1 = 1
1.5 = 15e-1
```
## Contact Author
You can reach me on the Nexus to provide bug reports or feedback https://www.nexusmods.com/valheim/mods/1042

For further mod or mod dev support, I can be found at the following Discord server:

[![](https://i.imgur.com/HZMpQip.png)](https://discord.gg/89bBsvK5KC)

## Config and Other Info:
Mod is highly configurable, a config file will be generated after first loading the mod and can be found in ﻿BepInEx/config/advize.PlantEverything.cfg

The config can be edited out of game with a text editor, or modified in game using the Configuration Manager mod.

## Config
### Default Config File:
```
Please see Nexus mod page for the default configuration.
```
## Source
Github Repo: [Advize_ValheimMods](https://github.com/AdvizeGH/Advize_ValheimMods)

## Screenshots

Showcase of some the additional flora added in 1.4.0

![](https://staticdelivery.nexusmods.com/mods/3667/images/1042/1042-1619617919-1974000660.png)

Added cultivator recipes

![](https://staticdelivery.nexusmods.com/mods/3667/images/1042/1042-1653289490-629916861.png)

Custom meshes for picked flowers and mushrooms, with growth time displayed

![](https://staticdelivery.nexusmods.com/mods/3667/images/1042/1042-1650757157-636832645.png)