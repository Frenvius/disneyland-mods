
# TeleportEverything
 > Produced by: Kpro and Elg

![](https://staticdelivery.nexusmods.com/mods/3667/images/1806/1806-1647282849-1161973402.png)

## About

This mod adds extra excitement and functionality to the portal system. You can use it to bring wolves to the fight or lure trolls into a trap! These modes also work in dungeons, so it's possible to bring a wolf into a mountain cave or have a wraith follow you into the crypt.

It's recommended to Install a [BepInEx Configuration Manager](https://valheim.thunderstore.io/package/Azumatt/Official_BepInEx_ConfigurationManager/) to change mod configurations in game using the `F1` key.

### **Important**
  1. Install on both server and clients for better use
  2. ServerSynched settings can only be changed by the server owner

> Note: There are some settings that only appear when you enable the advanced options in your configuration manager.

## Want to teleport faster?
Try using also the [QuickTeleport mod](https://valheim.thunderstore.io/package/OdinPlus/QuickTeleport/). It works perfectly with teleport everything and several other mods.

## Features

### Teleport Modes:

**All Teleport Modes allows you to teleport allies** and select your transport **Ally Mode**(tamed, named, only follow...). Read the documentation bellow to see all modes.

1. **Standard**. 
    Vanilla portal behavior.

2. **Vikings don't run**. 

    If this mode is selected from the **F1** configuration manager menu, portals will not work with enemies nearby. This makes escaping combat through portals more challenging, but not impossible.

3. **Take them with you**. 

    If this mode is selected from the **F1** configuration manager menu, enemies within the search range will have a chance of following you through the portal. Set the search range to a high number and watch out!

## Usage:

### **Message Mode**
* Change display message mode: 
    1. top left
    2. center
    3. none

### **--- Portal Settings ---**
* Portal Activation Range (advanced): You can increase or reduce the activation range. The default game value is 5 meters.
* Portal Sound Volume: Change between 0 and 100%. The default game value is 80%. You may need to rejoin the session or teleport to a distant portal for changes to take effect.

### **--- Portal Behavior ---**
#### Teleport Mode
1. Select the teleport mode: Currently you can select "**Standard**" which will give you vanilla behavior.  "**Vikings don't run**" mode will prevent you from teleporting if mobs are within a search sphere. "**Take them with you**" will give mobs a chance of following you through the portal. If this mode is selected, a dash through the portal with a troll in pursuit may end up in troll fight within your base! Its a super fun mode.
2. Currently, enemies will spawn at a random location within 6 meters (default) of the portal.

 Hey, if you want to bring some greydwarves through the portal with you, no one will judge ;). You can bring hostile creatures as easily as tamed ones.

 #### Search Radius (advanced)
 * Configurable search radius for creatures in meters, found in the F1 configuration menu.

___

### **--- Transport Allies ---**

#### Ally Mode
 If this mode is toggled on, allies within the search range will teleport with you. This includes wolves, boars, lox, or any creature. 

* Define the Ally Mode from the dropdown list using the **F1** configuration menu. At present, you can select either: 
  1. "No Allies",
  2. "All Tamed", 
  3. "Only Follow", 
  4. "All tamed except Named", 
  5. "Only Named".

> There are quick check boxes to select wolves, boar, or lox. You can also advanced filter which allies can be teleported by enabling the filter mask and entering the creature's prefab name (e.g. "greydwarf,wolf"). (In this case, only Greydwarfs and wolves allies would be allowed). You can obtain the prefab names list easily on the web.

#### Transport Radius and Vertical Tolerance (advanced)
* Teleport Everything searches for allies within a search cylinder. It should not be necessary but you can configure the radius and height of the search cylinder to meet your needs. For example, you might set the height to 1.5 meters in order to avoid transporting allies on different levels of your base.

#### Spawn Forward Tolerance (advanced)
* Define how far your allies will spawn in front of you in meters. The default is 1.5 meters.

#### User Filter Mask / Server Filter Mask (advanced)
* Enable Server/Player Filter Mask (advanced): 
    * If enabled, **only** allies in the Transport Mask field will be allowed
    * If disabled, **all tameable** allies can be teleportable
* Server and Player Transport Masks (advanced): accepts comma-delimited list of [prefab names](https://valheim-modding.github.io/Jotunn/data/prefabs/character-list.html). E.g.: wolf,lox (you can also use regex inside this field, e.g.: `human_\w+` will allow all `human_1`,`human_2`,`human_anything`).

#### Transport Boars / Lox / Wolves
* Three checkboxes that players can quickly enable/disable teleporting each creature. Default: all allowed.

___
### **--- Transport Carts ---** (advanced)

![transport-carts-gif](https://user-images.githubusercontent.com/101152506/220641406-59b27b02-25e9-4737-8b40-ce802c4b1a39.gif)

#### Transport Cart Mode
Choose between `Enabled`, `Disabled` and `Only Dungeons`. Synched with the server. Your player needs to be attached to the cart to transport it.

#### Transport Cart Tax Items
If Trasport Cart is enabled, switch on/off taking fee from prohibited cart items. It uses the Transport Fee configured on the server.

___
### **--- Transport Enemies ---** (advanced)
* These enemies settings are only appliable if "**Take Enemies With You**" is selected in the **Teleport Mode**.

#### Spawn Enemies Forward Tolerance
* The minimum distance enemies will spawn in front of you when teleported. Default 6 meters.

#### Max Enemy Spawn Radius
* The maximum radius enemies will spread in front of you when teleported. Default 3 meters.

#### Enemies Mask Mode
* Choose between **Disabled, Block or Allow Only** to use the Enemies Mask field.

#### Enemies Mask
* Write the prefab names of the enemies you want to follow/block, separated by a comma, depending on the Enemies Mask Mode.
___
### **--- Transport Items ---**
#### Transport Dragon Eggs / Transport Ores
* If toggled on, players can transport **ores, ingots, and eggs**. 

#### Transport fee (advanced)
* In order to offset the advantage of transporting ores, players may set a **"transport fee"** that deducts a percentage of the transported ores, ingots. For example, a 10% fee would take 3 out of 30 ores. Default: 0%.
* Dragon eggs are not taxed by default, but you can change it in the Remove Fee field.

#### Remove Transport Fee From Items (advanced)
* You can use the field to Remove the transport fee from specific items using their [prefab names](https://valheim-modding.github.io/Jotunn/data/prefabs/prefab-list.html). 
By default, the fee from `DragonEgg` is removed, but you can change it if needed.

* Advanced: [Regex expressions](https://regexr.com/70okv) are allowed, for example `boss_crystal_\w+` will remove the fee from any `boss_crystal_1`,`boss_crystal_2`,`boss_crystal_999`... (we automatically add a regex `\b` in the beggining and end to delimit the strings separated by comma)

<h2>Translations
  <img width="32" src="https://raw.githubusercontent.com/catamphetamine/country-flag-icons/master/3x2/US.svg" alt="English"/>
  <img width="32" src="https://raw.githubusercontent.com/catamphetamine/country-flag-icons/master/3x2/FR.svg" alt="French"/>
  <img width="32" src="https://raw.githubusercontent.com/catamphetamine/country-flag-icons/master/3x2/DE.svg" alt="German"/>
  <img width="32" src="https://raw.githubusercontent.com/catamphetamine/country-flag-icons/master/3x2/BR.svg" alt="Portuguese_Brazilian"/>
  <img width="32" src="https://raw.githubusercontent.com/catamphetamine/country-flag-icons/master/3x2/RU.svg" alt="Russian"/>
  <img width="32" src="https://raw.githubusercontent.com/catamphetamine/country-flag-icons/master/3x2/ES.svg" alt="Spanish"/>
</h2>

If you want to add your own translation locally, you can create a file based on the [English.yml template](https://cdn.discordapp.com/attachments/957320383424503949/1040075435674968094/English.yml) anywhere inside the Bepinex folder. The file should be named `TeleportEverything.Language.yml`. For example, the file for Spanish translation would be `TeleportEverything.Spanish.yml`.

You can find Valheim's Languages list [here](https://valheim-modding.github.io/Jotunn/data/localization/language-list.html).

### Built-in translations
Currently we have these translations in the mod: `English, French, German, Portuguese_Brazilian, Russian and Spanish`. You can send me your translation on odin plus discord if you want it added to the mod and available to other players in a later version.

## Installation Notes

1. Install this mod using your Mod Manager
2. Install BepInEx Configuration Manager: https://valheim.thunderstore.io/package/Azumatt/Official_BepInEx_ConfigurationManager/ (This mod will enable you to access the configuration settings simply by hitting **F1** and editting your mods configs in game)

> You can also define the configuration settings directly in the cfg file which is generated after the first run. (BepInEx/config/com.kpro.TeleportEverything.cfg)

## Manual Installation (Without Mod Manager)

1. Install *BepinEx* per the instructions at: https://valheim.thunderstore.io/package/denikson/BepInExPack_Valheim/

2. Install BepInEx Configuration Manager from: https://valheim.thunderstore.io/package/Azumatt/Official_BepInEx_ConfigurationManager/

3. Place ***TeleportEverything.dll*** into your **Bepinex\plugins** folder in Valheim.

## Dependencies

The mod requires two dependencies to work properly:

* BepInEx Valheim (Mandatory)
* BepInEx Configuration Manager (Recommended)

## Mod Compatibility

The mod is compatible with several other mods and we are always improving it.

- ![YES]: [QuickTeleport](https://valheim.thunderstore.io/package/OdinPlus/QuickTeleport/)
- ![YES]: Basement or BasementJVLedition
- ![YES]: Jewelcrafting
  - If you don't want to tax boss crystals, you can add to the Remove Transport fee field the  following boss crystal regex: `Boss_Crystal_\w+`
  - Separate by comma if you want to remove from other items, e.g.: `Boss_Crystal_\w+,DragonEgg`
- ![YES]: MapTeleport
- ![YES]: OdinsUndercroft
- ![YES]: Skyheim
- ![YES]: TargetPortal
- ![YES]: Wayshrine
- ![YES]: AllTameableHandH
  - (If your vertical tolerance is low, you may not be able to transport a flying drake)
- ![PARTIAL]: UnrestrictedPortals
  - You can use the ore configs from UnrestrictedPortals if you disable Teleport Ore or Dragon Eggs checkboxes from TeleportEverything config.
  - Item Fees don't work if you are using UnrestrictedPortals configs.

<p>
  <p align="center"><h2>For Questions or Comments find Elg or KPro in the Odin Plus Team on Discord:</h2></p>

  <p align="center"><a href="https://discord.gg/mbkPcvu9ax"><img src="https://i.imgur.com/Ji3u63C.png" alt="Odin Plus Discord"></a>
</p>

## Changelog
- Version 2.5.1
  - Valheim update - server sync fix
- Version 2.5.0
  - Valheim Hildir's Request Update
- Version 2.4.0
  - Valheim update fix
- Version 2.3.1
  - Performance improvement (Thanks to @CW-Jesse)
  - Increased default ally spawn forward value to 1.5 meters
- Version 2.3.0
  - Transport carts and charge an optional fee
  - Toggle teleport animation screen on/off
- Version 2.2.0
  - Added a mask to block/allow only specific enemies to be teleported
  - Fixed bug that allowed unalerted enemies to be teleported
- Version 2.1.0
  - Mistlands update
- Version 2.0.0
  - Added translations in French, German, Portuguese_Brazilian, Russian and Spanish
- Version 1.9.0
  - Added compatibility to Skyheim
  - Fixed allies and enemies messages
  - Fixed inventory/crafting UI
- Version 1.8.0
  - Items in inventory now shows transport fee value. Non-teleportable icon removed accordingly
  - Added partial compatibility with UnrestrictedPortals
  - Changed default values for easier mod setup
  - Fixed Masks and added a field to avoid prohibited items from being taxed
  - Added Regex match for masks/remove fee fields
  - Updated ServerSync
- Version 1.7.0
  - Added tax compatibility with TargetPortal mod
- Version 1.6.2
  - Fixed tax to deduct from total number of ores instead of each stack
  - Fixed tax to apply to quantities less than the tax amount
- Version 1.6.1
  - Add height check to prevent creatures from getting stuck in crypts
- Version 1.6
  - Added Server Sync (compatible with servers and clients)
  - Separated Server and Player Filter Mask (if mask disabled, all allies can be transported)
  - Removed delayed spawn
  - Removed fee for disconnected portals
  - Fixed spawn offset
  - Fixed teleport with enemies
- Version 1.5
  - Added delayed spawn to allies and enemies (single player)
  - Added sound volume and activation range options for portals
  - Added advanced settings (if you need more options, enable config manager advanced mode)
- Version 1.4
  - Added transport of ores, ingots, and eggs.
  - Added optional "transport fee" that reduces ore, ingots, and eggs as a fee for transport these items
  - Added configurable settings for fee feature
- Version 1.3
  - Added display messages top left, center, or none
  - Fixed teleport bug out of sunken crypts
  - Added configurable spawn location for allies
  - Mask now accepts comma-delimited list, ignoring case and white space.
- Version 1.2
  - Fixed error in vertical distance calculation. 
  - Fixed error in determining named boars or wolves.
- Version 1.1
  - Update adds control over transport mechanic including search radius and limiting transport to tamed, named, followed, etc.
- Version 1.0
  - Alpha-version of the mod. Feedback and bug reports appreciated.

[YES]: https://img.shields.io/badge/YES-success?style=flat-square
[PARTIAL]: https://img.shields.io/badge/PARTIAL-yellow?style=flat-square