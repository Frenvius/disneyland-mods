### Loot Multiplier for Valheim - DropMoreLoot

This is a rebirth of Castix's Loot Multiplier mod.  Redone with permission from Castix  (SoCastix)      
Castix no longer had the source and gave me permission to rebuild it, add features and release to the gaming community.  

Credit to Castix for the original idea and awesome mod "Loot Multiplier".




> ### This mod does the following:

> - multiplies loot drops when you destroy, kill or pick up something. Drop multiplier can be configured.  
 
> - floating loot
> - configurable pickup range
> - item stacking
> - configurable whitelist - see below
___
### This mod is incompatible with Creature Level and Loot Control (CLLC) - Which is an amazing mod

Most, if not all of this mod's features are included in CLLC.  That being said, I've always liked the simplicity of this mod and have no desire to alter creature levels or need the sheer depth of settings and features that CLLC provides.
`Use this mod and CLLC at your own risk.` 

___
Installation (manual)                                                                                       

If you are installing this manually, do the following
1. Extract the archive into a folder. **Do not extract into the game folder.**
2. Move the contents of `plugins` folder into `<GameDirectory>\Bepinex\plugins`.
3. Run the game.
4. To change the drop rate, use the config at \BepInEx\config\TastyChickenLegs.DropMoreLoot.cfg


How to set up the custom whitelist

1. Enable the whitelist in the Loot Multiplier config.
2. Open the whitelist.txt file. It always has to be in the same directory as the plugin .dll (example: <GameDirectory>\BepInEx\plugins\LootMultiplier\whitelist.txt)
3. Add items to the list by writing the Prefab name of the item you want. One per line.
4. If the whitelist is enabled, only the allowed items inside it will be multiplied.

Prefab names list:
Item List from Reddit
Item List from Modding Wiki﻿﻿


﻿

![Configuration](https://i.ibb.co/WPMrK8w/lootsmall.png)
### Configuration:                                                     



Material Multiplier
- Setting type: Int32
- Default value: 3
- Multiplier for resources = 1-5

Monster Drop Multiplier
- Setting type: Int32
- Default value: 3
- Multiplier for monster drops = 1-5

Pickup Multiplier
- Setting type: Int32
- Default value: 3
- Multiplier for pickable objects = 1-5


Items Float in Water

- Default value: true
- Enable Items to float in water

Stacking

- Default value: true
- Enable Items to stack

Pickup radius

- Default value: 3
- Configure distance items are automatically picked up. 1-10

![White List](https://i.imgur.com/a1uSfeB.png)

[Whitelist]

Whitelist
- Setting type: Boolean
- Default value: false
- Enable whitelist filter = false
_____________

### Versions:

1.0.5

- fixed incompatiblity issues with other mods.

1.0.4

- increased allowable distance to 10

1.0.3

- fix for resources multiplier

1.0.2

- fix for tree chopping null exception

1.0.0

- Initial Release

_____
##	Now for the shameless plug

> ### My Other Mods:
>>* [No Smoke Stay Lit](https://valheim.thunderstore.io/package/TastyChickenLeg/NoSmokeStayLit/)
>>* [No Smoke Simplified](https://valheim.thunderstore.io/package/TastyChickenLegs/NoSmokeSimplified/)
>>* [Honey Please](https://valheim.thunderstore.io/package/TastyChickenLegs/HoneyPlease/)
>>* [Automatic Fuel](https://valheim.thunderstore.io/package/TastyChickenLeg/AutomaticFuel/)
>>* [Forsaken Powers Plus](https://valheim.thunderstore.io/package/TastyChickenLeg/ForsakenPowersPlus/)
>>* [Recycle Plus](https://valheim.thunderstore.io/package/TastyChickenLeg/RecyclePlus/)
>>* [Blast Furnace Takes All](https://valheim.thunderstore.io/package/TastyChickenLeg/BlastFurnaceTakesAll/)
>>* [Timed Torches Stay Lit](https://valheim.thunderstore.io/package/TastyChickenLeg/TimedTorchesStayLit/)