# Description

This mod pulls nearby items from the ground into containers. Optionally, use a hotkey to store items in your inventory
into containers. WardIsLove compatible, HotBar items can be ignored (on by default), Quickslots can be
ignored (`if turned on in the configuration!`).

## 1. Need to know

`Version checks with itself. If installed on the server, it will kick clients who do not have it installed.`

`This mod uses ServerSync, if installed on the server and all clients, it will sync all configs to client`

`This mod uses a file watcher. If the configuration file is not changed with BepInEx Configuration manager, but changed in the file directly on the server, upon file save, it will sync the changes to all clients.`

## Features

- Automatically store dropped resources into nearby containers within a configurable range
- Restrict specific items from being stored into containers by defining rules in the configuration file in
  the `BepInEx/config` folder called `Azumatt.AzuAzuStore.yml`
- Toggle the storing of items via a keyboard shortcut for a configurable amount of seconds

## FAQ

- Frequently asked questions will be added to the wiki tab of this mod as they are asked. Wiki tab is located at the top
  of this page (or you can be lazy and click this here linky
  link: https://valheim.thunderstore.io/package/Azumatt/AzuAutoStore/wiki/).

## 2. Configuration (Collapsed due to length. Click to expand)

<details> <summary><b>Available Configuration Options</b></summary>




`1 - General`

Lock Configuration [Synced with Server]

* If on, the configuration is locked and can be changed by server admins only.
    * Default Value: On

Must Have Existing Item To Pull [Synced with Server]

* If on, the chest must already have the item in its inventory to pull it from the world or player into the chest.
    * Default Value: Off

Player Range [Synced with Server]

* The maximum distance from the player to store items in chests when the Store Shortcut is pressed. Follows storage
  rules for allowed items.
    * Default Value: 5

Fallback Range [Synced with Server]

* The range to use if the container has no range set in the yml file. This will be the fallback range for all
  containers.
    * Default Value: 10

Player Ignore Hotbar [Not Synced with Server]

* If on, the player's hotbar will not be stored when the Store Shortcut is pressed.
    * Default Value: On

Player Ignore Quick Slots [Not Synced with Server]

* If on, the player's quick slots will not be stored when the Store Shortcut is pressed. (Requires Quick Slots mod, turn
  on only if you need it!)
    * Default Value: Off

Ping VFX [Synced with Server]

* The VFX to play when a chest is pinged. Leave blank to disable and only highlight the chest. (Full prefab
  list: https://valheim-modding.github.io/Jotunn/data/prefabs/prefab-list.html)
    * Default Value: vfx_Potion_health_medium

Highlight Containers [Not Synced with Server]

* If on, the containers will be highlighted when something is stored in them. If off, the containers will not be
  highlighted if something is stored in them.
    * Default Value: On

Seconds To Wait Before Storing [Synced with Server]

* The number of seconds to wait before storing items into chests nearby automatically after you have pressed your hotkey
  to pause.
    * Default Value: 10

`2 - Shortcuts`

Store Shortcut [Not Synced with Server]

* Keyboard shortcut/Hotkey to store your inventory into nearby containers.
    * Default Value: Period

Pause Shortcut [Not Synced with Server]

* Keyboard shortcut/Hotkey to temporarily stop storing items into chests nearby automatically. Does not override the
  player hotkey store.
    * Default Value: LeftShift + Period

</details>


<details>
<summary><b>Installation Instructions</b></summary>

### Manual Installation

`Note: (Manual installation is likely how you have to do this on a server, make sure BepInEx is installed on the server correctly)`

1. **Download the latest release of BepInEx.**
2. **Extract the contents of the zip file to your game's root folder.**
3. **Download the latest release of AzuAutoStore from Thunderstore.io.**
4. **Extract the contents of the zip file to the `BepInEx/plugins` folder.**
5. **Launch the game.**

### Installation through r2modman or Thunderstore Mod Manager

1. **Install [r2modman](https://valheim.thunderstore.io/package/ebkr/r2modman/)
   or [Thunderstore Mod Manager](https://www.overwolf.com/app/Thunderstore-Thunderstore_Mod_Manager).**

   > For r2modman, you can also install it through the Thunderstore site.
   ![](https://i.imgur.com/s4X4rEs.png "r2modman Download")

   > For Thunderstore Mod Manager, you can also install it through the Overwolf app store
   ![](https://i.imgur.com/HQLZFp4.png "Thunderstore Mod Manager Download")
2. **Open the Mod Manager and search for "AzuAutoStore" under the Online
   tab. `Note: You can also search for "Azumatt" to find all my mods.`**
   The image below shows VikingShip as an example, but it was easier to reuse the image. Type AzuAutoStore.

![](https://i.imgur.com/5CR5XKu.png)

3. **Click the Download button to install the mod.**
4. **Launch the game.**

</details>



<details><summary><b>Example YAML</b></summary>

```yaml
# Below you can find example groups. Groups are used to exclude or includeOverride quickly. They are reusable lists! 
# Please note that some of these groups/container limitations are kinda pointless but are here for example.
# Make sure to follow the format of the example below. If you have any questions, please ask in my discord.

# Full vanilla prefab name list: https://valheim-modding.github.io/Jotunn/data/prefabs/prefab-list.html
# Item prefab name list: https://valheim-modding.github.io/Jotunn/data/objects/item-list.html

# There are several predefined groups set up for you that are not listed. You can use these just like you would any group you create yourself.
# These are the "All", "Food", "Potion", "Fish", "Swords", "Bows", "Crossbows", "Axes", "Clubs", "Knives", "Pickaxes", "Polearms", "Spears", "Equipment", "Boss Trophy", "Trophy", "Crops", "Seeds", "Ores", "Metals", and "Woods" groups.
# The criteria for these groups are as follows:
# groups:
#   Food:
#     - Criteria: Both of the following properties must have a value greater than 0.0 on the sharedData property of the ItemDrop script:
#         - food
#         - foodStamina
#   Potion:
#     - Criteria: The following properties must meet the specified conditions on the sharedData property of the ItemDrop script:
#         - food > 0.0
#         - foodStamina == 0.0
#   Fish:
#     - itemType: Fish
#   Swords, Bows, Crossbows, Axes, Clubs, Knives, Pickaxes, Polearms, Spears:
#     - itemType: OneHandedWeapon, TwoHandedWeapon, TwoHandedWeaponLeft, Bow
#     - Criteria: Items in these groups have a specific skillType on the sharedData property of the ItemDrop script. Each group corresponds to the skillType as follows:
#         - Swords: skillType == Skills.SkillType.Swords
#         - Bows: skillType == Skills.SkillType.Bows
#         - Crossbows: skillType == Skills.SkillType.Crossbows
#         - Axes: skillType == Skills.SkillType.Axes
#         - Clubs: skillType == Skills.SkillType.Clubs
#         - Knives: skillType == Skills.SkillType.Knives
#         - Pickaxes: skillType == Skills.SkillType.Pickaxes
#         - Polearms: skillType == Skills.SkillType.Polearms
#         - Spears: skillType == Skills.SkillType.Spears
#            Example:   An item with itemType set to OneHandedWeapon and skillType set to Skills.SkillType.Swords would belong to the Swords group.
#   Equipment:
#     - itemType: Torch
#   Boss Trophy:
#     - itemType: Trophy
#     - Criteria: sharedData.m_name ends with any of the following boss names:
#         - eikthyr, elder, bonemass, dragonqueen, goblinking, SeekerQueen
#   Trophy:
#     - itemType: Trophy
#     - Criteria: sharedData.m_name does not end with any boss names
#   Crops:
#     - itemType: Material
#     - Criteria: Can be cultivated and grown into a pickable object with an amount greater than 1
#   Seeds:
#     - itemType: Material
#     - Criteria: Can be cultivated and grown into a pickable object with an amount equal to 1
#   Ores:
#     - itemType: Material
#     - Criteria: Can be processed by any of the following smelters:
#         - smelter
#         - blastfurnace
#   Metals:
#     - itemType: Material
#     - Criteria: Is the result of processing an ore in any of the following smelters:
#         - smelter
#         - blastfurnace
#   Woods:
#     - itemType: Material
#     - Criteria: Can be processed by the charcoal_kiln smelter
#   All:
#     - Criteria: Item has an ItemDrop script and all needed fields are populated. (all items)




groups:
  Armor: # Group name
    - ArmorBronzeChest # Item prefab name, note that this is case sensitive and must be the prefab name
    - ArmorBronzeLegs
    - ArmorCarapaceChest
    - ArmorCarapaceLegs
    - ArmorFenringChest
    - ArmorFenringLegs
    - ArmorIronChest
    - ArmorIronLegs
    - ArmorLeatherChest
    - ArmorLeatherLegs
    - ArmorMageChest
    - ArmorMageLegs
    - ArmorPaddedCuirass
    - ArmorPaddedGreaves
    - ArmorRagsChest
    - ArmorRagsLegs
    - ArmorRootChest
    - ArmorRootLegs
    - ArmorTrollLeatherChest
    - ArmorTrollLeatherLegs
    - ArmorWolfChest
    - ArmorWolfLegs
  Arrows:
    - ArrowBronze
    - ArrowCarapace
    - ArrowFire
    - ArrowFlint
    - ArrowFrost
    - ArrowIron
    - ArrowNeedle
    - ArrowObsidian
    - ArrowPoison
    - ArrowSilver
    - ArrowWood
    - draugr_arrow
  Tier 2 Items:
    - Bronze
    - PickaxeBronze
    - ArmorBronzeChest
    - ArmorBronzeLeggings


# By default, if you don't specify a container below, it will be considered as you want to allow storing all objects into it.
# If you are having issues with a container, please make sure you have the full prefab name of the container. Additionally, make sure you have range and exclude or includeOverride set up correctly.
# Worst case you can define a container like this. This will allow everything to be pulled from the container within a range of 30.
# rk_barrel:  
#   range: 30
#  includeOverride: []

## Please note that the below containers are just examples. You can add as many containers as you want.
## If you want to add a new container, just copy and paste the below example and change the name of the container to the prefab name of the container you want to add.
## The values are set up to include everything by using the includeOverride (aside from things that aren't really a part of vanilla recipes, like Swords or Bows). 
## This is to give you examples on how it's done, but still allow everything to be stored into the container.

piece_chest:
  range: 10 # This is the range that the container will store items. This overrides the global range set in the config.
  exclude: # Exclude these items from being able to be stored into the container
    #- Food # Exclude all in group
    - PickaxeBronze # Allow prefab names as well, in this case we will use something that isn't a food
  includeOverride:
    # - Food # This would not work, you cannot includeOverride a group that is excluded. You can only override prefabs from that group.
    - PickaxeBronze # You can however, be weird, and override a prefab name you have excluded.

# It's highly unlikely that you will need the armor, swords, bows, etc. groups below. These are just in case you want to use them. 
# They were also easy ways for me to show you how to use the groups without actually excluding something you might want to always pull by default.

piece_chest_wood:
  range: 10
  exclude:
    - Swords # Exclude all in group
    - Tier 2 Items # Exclude all in group
    - Bows # Exclude all in group
  includeOverride: # If the item is in the groups above, say, you were using a predefined group but want to override just one item to be ignored and allow pulling it
    - BowFineWood
    - Wood
    - Bronze
    - PickaxeBronze
    - ArmorBronzeChest
    - ArmorBronzeLeggings

piece_chest_private:
  range: 10
  exclude:
    - All # Exclude everything

piece_chest_blackmetal:
  range: 10
  exclude:
    - Swords # Exclude all in group
    - Tier 2 Items # Exclude all in group
    - Bows # Exclude all in group
  includeOverride: # If the item is in the groups above, say, you were using a predefined group but want to override just one item to be ignored and allow storing it
    - BowFineWood
    - Wood
    - Bronze

rk_cabinet: # rk_ is typically the prefix for containers coming from RockerKitten's mods
  range: 10
  exclude:
    - Food
  includeOverride:
    - Food

rk_cabinet2:
  range: 10
  exclude:
    - Food
  includeOverride:
    - Food

rk_barrel:
  range: 10
  exclude:
    - Armor
    - Swords

rk_barrel2:
  range: 10
  exclude:
    - Armor
    - Swords

rk_crate:
  range: 10
  exclude:
    - Armor
    - Swords

rk_crate2:
  range: 10
  exclude:
    - Armor
    - Swords
```

</details>


`Feel free to reach out to me on discord if you need manual download assistance.`

# Author Information

### Azumatt

`DISCORD:` Azumatt#2625

`STEAM:` https://steamcommunity.com/id/azumatt/

For Questions or Comments, find me in the Odin Plus Team Discord or in mine:

[![https://i.imgur.com/XXP6HCU.png](https://i.imgur.com/XXP6HCU.png)](https://discord.gg/Pb6bVMnFb2)
<a href="https://discord.gg/pdHgy6Bsng"><img src="https://i.imgur.com/Xlcbmm9.png" href="https://discord.gg/pdHgy6Bsng" width="175" height="175"></a>