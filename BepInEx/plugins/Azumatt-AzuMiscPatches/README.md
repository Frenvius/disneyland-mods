# Description

## Collection of patches from OdinQOL that didn't really have a home in a mod of their own


`Version checks with itself. If installed on the server, it will kick clients who do not have it installed.`

`This mod uses ServerSync, if installed on the server and all clients, it will sync all configs with [Synced with Server] to client`

`This mod uses a file watcher. If the configuration file is not changed with BepInEx Configuration manager, but changed in the file directly on the server, upon file save, it will sync the changes to all clients.`


---

### Features

`1 - General`

Lock Configuration [Synced with Server]
* If on, the configuration is locked and can be changed by server admins only.
    * Default Value: On

`2 - Player`

Modify food [Synced with Server]
* Ensuring the food lasts longer while maintaining the same rate of regeneration. Needed to be on for No Food Degrade to work
    * Default Value: On

No Food Degrade [Synced with Server]
* Disable food degradation over time (maintain full benefit for the whole duration).
    * Default Value: On

Re Equip after Swimming [Not Synced with Server]
* Re-equip Items After Swimming
    * Default Value: On

`3 - Inventory & Items`

Item Weight Increase [Synced with Server]
* Multiplier for your item weight. This is a modifier value. 50 will increase it by 50%, -50 will reduce it by 50%.
    * Default Value: 1

Item Stack Increase [Synced with Server]
* Multiplier for your item stacks. Directly multiplies stack of the item by this value. (Stack of 50 with value of 10 here would turn into a stack of 500). Multiplier must be higher than 0 to apply.
    * Default Value: 1

Disable Teleport check for items [Synced with Server]
* Disable Teleport check for items
    * Default Value: Off

Fill Top to Bottom [Not Synced with Server]
* Move your things top to bottom when changing from inv to chest
    * Default Value: Off

Merge Stacks [Not Synced with Server]
* Merge stacks when moving items from inv to chest (or another inventory). Try to merge items with existing stacks.
    * Default Value: Off

`4 - Game`

Portal Character Limit [Synced with Server]
* Removes the character limit for portals. Default value of Vanilla is 10 characters
  * Default Value: Off
  
No Minimum Password Length [Synced with Server]
* No Minimum password length for server
    * Default Value: On

Mute Game in Background [Not Synced with Server]
* Mute the game when you alt tab out of it, or it loses focus.
    * Default Value: On

I have arrived disable [Synced with Server]
* Disable the I have arrived message
    * Default Value: On

BuildInProtectedLocations [Synced with Server]
* Allow Building Inside Protected Locations
    * Default Value: Off

Ignore space restrictions [Synced with Server]
* Ignore space restrictions. This will allow you to build pieces close together.
    * Default Value: Off

Disable Guardian Animation [Synced with Server]
* Disable Guardian Animation for the players
    * Default Value: Off

Skip Tuts [Not Synced with Server]
* Skip Tutorials
    * Default Value: Off

Honey Speed [Synced with Server]
* Honey Production Speed
    * Default Value: 1200

Honey Count Per Hive [Synced with Server]
* Honey Count Per Hive
    * Default Value: 4

`5 - Building HUD`

Can Build Amount Format [Not Synced with Server]
* Format for the amount of times you can build the currently selected item with your current inventory. Uses standard C# format rules. Leave empty to hide altogether.
    * Default Value: ({0})

Can Build Amount Color [Not Synced with Server]
* Color to set the can-build amount. Leave empty to set no color. You can use the #XXXXXX hex color format.
    * Default Value: white


---



`Feel free to reach out to me on discord if you need manual download assistance.`


# Author Information

### Azumatt

`DISCORD:` Azumatt#2625

`STEAM:` https://steamcommunity.com/id/azumatt/

For Questions or Comments, find me in the Odin Plus Team Discord or in mine:

[![https://i.imgur.com/XXP6HCU.png](https://i.imgur.com/XXP6HCU.png)](https://discord.gg/Pb6bVMnFb2)
<a href="https://discord.gg/pdHgy6Bsng"><img src="https://i.imgur.com/Xlcbmm9.png" href="https://discord.gg/pdHgy6Bsng" width="175" height="175"></a>