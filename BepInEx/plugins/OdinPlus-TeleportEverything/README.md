
# TeleportEverything
 > Produced by: Kpro and Elg

![](https://staticdelivery.nexusmods.com/mods/3667/images/1806/1806-1647282849-1161973402.png)

## About

This mod is intended to add additional excitement and functionality to the portal system. Use it to brings wolves to the fight or use it to lure trolls into a trap!  These modes also work with dungeons! So its possible to bring a wolf into a swamp crypt and for a wraith to follow you into the crypt!

It's recommended to Install a [BepInEx Configuration Manager](https://valheim.thunderstore.io/package/Azumatt/Official_BepInEx_ConfigurationManager/) to be able to change mod configurations in game.

> Note: There are some settings that only appear when you enable the advanced options in your configuration manager.

## Did you like the mod? Buy me a coffee to support the development
<p align="center">
  <a href="https://www.buymeacoffee.com/elgthedev">
    <img width="300" alt="bmc-button" src="https://user-images.githubusercontent.com/101152506/215227016-c5a9ea72-fe35-42bf-be89-06c643b46993.png">
  </a>
</p>

## Features

### Modes:

1. **Standard**. 

    Vanilla behavior for portals except that you can still transport allies.

2. **Vikings don't run**. 

    If this mode is selected from the **F1** configuration manager menu, portals will not work with enemies nearby. It is intended to make a cowardly retreat through a portal in order to avoid combat a bit more challenging but not impossible.

3. **Take them with you**. 

    If this mode is selected from the **F1** configuration manager menu, enemies within the search range will have small chance of following you through the portal. Set the search range to a high number and watch out!

4. **Transport Allies**. 

    If this mode is toggled on, allies within the search range will teleport with you. You can teleport wolves, boar, lox, or anything creature at all. Hey, if you want to bring some greydwarves through the portal with you, no one will judge ;). The ally does not need to be tamed to transport so a hostile wolf or boar can come through as easily as a tamed wolf or boar.

## Usage:

### **Message Mode**
* You can change the display message mode between: top left, center, or none.

### **--- Portal Settings ---**
* Portal Activation Range(advanced): You can increase or reduce the activation range, 5 meters is the default game value.
* Portal Sound Volume: You can change it between 0 and 100%. 80% is the default game value.

### **--- Portal Behavior ---**
#### Teleport Mode
1. Select the teleport mode. Currently you can select "**Standard**" which will give you vanilla behavior.  "**Vikings don't run**" mode will prevent you from teleporting if mobs are within a search sphere. "**Take them with you**" will give mobs a chance of following you through the portal. If this mode is selected, a dash through the portal with a troll in pursuit may end up in troll fight within your base! Its a super fun mode.
2. At present, enemies will spawn at a random location forward within 6 meters (default) of the portal.

 #### Search Radius (advanced)
 * The search radius to search creatures in meters. It is configurable in the **F1** configuration menu.

___

### **--- Transport Allies ---**

#### Ally Mode
1. Define the ally type that you want to transport using the **F1** configuration menu. There quick check boxes to select wolves, boar, or lox. If you want to filter which animals can be teleportable, enable the filter mask and use the transport mask by typing in the spawn name of the creatures. An example would be "**Greydwarf**" without the quote marks. (In this case, only Greydwarfs would be allowed) You can obtain the list spawn names easily on the web.
2. Define the Ally Mode from the dropdown list. At present, you can select either: 
   * "No Allies",
   * "All Tamed", 
   * "Only Follow", 
   * "All tamed except Named", 
   * "Only Named".

#### Transport Radius and Vertical Tolerance (advanced)
* Teleport Everything will search for allies within a search cylinder. It should not be necessary but you can configure the radius and height of the search cylinder to meet your needs. For example, you might set the height to 1.5 in order to avoid transporting allies on different levels of your base.

#### Spawn Forward Tolerance (advanced)
* Defines how far your allies will spawn in your front in meters. Default 1 meter.

#### User Filter Mask / Server Filter Mask (advanced)
* Enable Server/Player Filter Mask (advanced): 
    * If enabled, **only** the allies in the Transport Mask field will be allowed
    * If disabled, **all tameable** allies can be teleportable
* Server and Player Transport Masks (advanced): accepts comma delimited list of [prefab names](https://valheim-modding.github.io/Jotunn/data/prefabs/character-list.html). E.g.: wolf,lox (you can also use regex inside this field, e.g.: `human_\w+` will allow all human_1,human_2,human_anything).

#### Transport Boars / Lox / Wolves
* There are 3 checkboxes that players can quickly enable/disable teleporting each creature. Default: all allowed.

___
### **--- Transport Enemies ---** (advanced)
* These enemies settings are only appliable if "**Take Enemies With You**" is selected in the **Teleport Mode**.
#### Spawn Enemies Forward Tolerance
* The min distance that enemies will spawn in front of you when teleported. Default 6 meters.

#### Max Enemy Spawn Radius
* The max radius that enemies will spread in front of you when teleported. Default 3 meters.

#### Enemies Mask Mode
* Choose between **Disabled, Block or Allow Only** to use the Enemies Mask field.

#### Enemies Mask
* Write separated by comma the prefab names of the enemies you want to follow/block following players depending on the Enemies Mask Mode.
___
### **--- Transport Items ---**
#### Transport Dragon Eggs / Transport Ores
* If toggled on, players may transport **ores, ingots, and eggs**. 

#### Transport fee (advanced)
* In order to offset the advantage of transporting ores, players may set a **"transport fee"** that deducts a percentage of the contraband ores, ingots. For example: a percentage of 10% would take 3 out of 30 ores. Default: 0%.
* Dragon eggs are not taxed by default, but you can change it in the Remove Fee field.

#### Remove Transport Fee From Items (advanced)
* You can use the field to Remove the transport fee from specific items using their [prefab names](https://valheim-modding.github.io/Jotunn/data/prefabs/prefab-list.html). 
By default the fee from the folowing item is removed: `DragonEgg` but you can change it if needed.

* Advanced: [Regex expressions](regexr.com/70okv) are allowed, for example `boss_crystal_\w+` will remove the fee from any boss_crystal_1,boss_crystal_2,boss_crystal_999... (we automatically add a `\b` in the beggining and end to delimit the strings separated by comma)

## Translations
If you want to add your own translation locally, you can create a file based on the [English.yml template](https://cdn.discordapp.com/attachments/957320383424503949/1040075435674968094/English.yml) anywhere inside of the Bepinex folder with the name: 
`TeleportEverything.Language.yml`. For example, the file for a Spanish translation would be: `TeleportEverything.Spanish.yml`

You can find Valheim's Languages list [here](https://valheim-modding.github.io/Jotunn/data/localization/language-list.html).

Currently we have these translations in the mod: `English, French, German, Portuguese_Brazilian, Russian and Spanish`. You can send me your translation on odin plus discord if you want it added to the mod and available to other players in a later version.

## Installation Notes

1. Install this mod using your Mod Manager
2. Install BepInEx Configuration Manager: https://valheim.thunderstore.io/package/Azumatt/Official_BepInEx_ConfigurationManager/ (This mod will enable you to access the configuration settings simply by hitting **F1** and editting your mods configs in game)

> You can also define the configuration settings directly in the cfg file which is generated after the first run. (BepInEx/config/com.kpro.TeleportEverything.cfg)

## Manual Installation (Without Mod Manager)

1. Install *BepinEx* per the author's instructions here: https://valheim.thunderstore.io/package/denikson/BepInExPack_Valheim/

2. Install BepInEx Configuration Manager: https://valheim.thunderstore.io/package/Azumatt/Official_BepInEx_ConfigurationManager/

3. Place ***TeleportEverything.dll*** into your **Bepinex\plugins** folder in valheim.

## Dependencies

To make it work properly you will need some other mods or tools called dependencies so make sure that everything is installed as it should. To make it work properly you need these dependencies:

* BepInEx Valheim (Mandatory)
* BepInEx Configuration Manager (Recommended)

## Mod Compatibility

- ![YES]: AllTameableHandH
  - (If your vertical tolerance is low, you may not be able to transport a flying drake)
- ![YES]: Basement or BasementJVLedition
- ![YES]: FastTeleport
- ![YES]: Jewelcrafting
  - If you don't want to tax boss crystals, you can add to the Remove Transport fee field the  following boss crystal regex: `Boss_Crystal_\w+`
  - Separate by comma if you want to remove from other items, e.g.: `Boss_Crystal_\w+,DragonEgg`
- ![YES]: MapTeleport
- ![YES]: OdinsUndercroft
- ![YES]: Skyheim
- ![YES]: TargetPortal
- ![YES]: Wayshrine
- ![PARTIAL]: UnrestrictedPortals
  - You can use the ore configs from UnrestrictedPortals if you disable Teleport Ore or Dragon Eggs checkboxes from TeleportEverything config.
  - Item Fees don't work if you are using UnrestrictedPortals configs.

<p>
  <p align="center"><h2>For Questions or Comments find Elg or KPro in the Odin Plus Team on Discord:</h2></p>

  <p align="center"><a href="https://discord.gg/mbkPcvu9ax"><img src="https://i.imgur.com/Ji3u63C.png"></a>
</p>

## Changelog
- Version 2.2.0
  - Added a mask to block/allow teleporting enemies
  - Fixed unalerted enemies being teleported
- Version 2.1.0
  - Mistlands update
- Version 2.0.0
  - Added translations (French, German, Portuguese_Brazilian, Russian and Spanish)
- Version 1.9.0
  - Added compatibility to Skyheim
  - Fixed allies and enemies messages
  - Fixed inventory/crafting UI
- Version 1.8.0
  - Items in inventory now show transport fee value. Non-teleportable icon removed accordingly
  - Added partial compatibility to UnrestrictedPortals
  - Changed the default values to make the mod setup easier
  - Fixed Masks and added a field to avoid prohibited items from being taxed
  - Added Regex match to the masks/remove fee fields
  - Updated ServerSync
- Version 1.7.0
  - Added tax compatibility when using TargetPortal mod
- Version 1.6.2
  - Fixed tax to deduct from total number of ores instead of each stack
  - Fixed tax to apply also to quantities less than the tax
- Version 1.6.1
  - Add height check to prevent creatures from getting stuck in crypts
- Version 1.6
  - Added Server Sync (Now compatible with servers and clients)
  - Separated Server and Player Filter Mask (if mask is not enabled, all allies can be transported)
  - Removed delayed spawn
  - Removed fee on disconnected portals
  - Spawn offset fixed
  - Teleport with enemies fixed
- Version 1.5
  - Added delayed spawn to allies and enemies (single player)
  - Added settings to change portal sound volume and activation range
  - Added advanced settings (if you need more options, enable config manager advanced mode)
- Version 1.4
  - Added transport of ores, ingots, and eggs.
  - Added optional "transport fee" that reduces ore, ingots, and eggs as a fee for transport these "contraband" items.
  - Added configurations settings for this feature.
- Version 1.3
  - Added display messages top left, center, or none
  - Fixed teleport bug out of sunken crypts
  - Added configurable spawn location for allys
  - Transport mask now accepts comma delimited list. Ignores case and white space.
- Version 1.2
  - Fixed error in calculation of vertical distance. Fixed error determine whether boars or wolves are named.
- Version 1.1
  - Update provides additional control over transport mechanic including control over the search radius and ability to limit transport to tamed, named, follow, etc.
- Version 1.0
  - This is the alpha-version of the mod. Feedback and bug reports are appreciated.

[YES]: https://img.shields.io/badge/YES-success?style=flat-square
[PARTIAL]: https://img.shields.io/badge/PARTIAL-yellow?style=flat-square