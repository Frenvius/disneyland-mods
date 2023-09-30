# Description

<img src="https://github.com/AzumattDev/Recycle_N_Reclaim/assets/80414405/69371c0f-d56a-4019-807b-13696778a1f1" alt="5B0B26B8-8064-421E-8888-6D40E71C56DC-min" width="100%" style="max-width: 1280px; height: auto;">

## A mod that allows you to recycle/reclaim items back into resources used to make them. Adds a 'Reclaim' tab/button to the crafting menu. Additionally can be used inside of your inventory directly.

`Version checks with itself. If installed on the server, it will kick clients who do not have it installed.`

`This mod uses ServerSync, if installed on the server and all clients, it will sync all configs to client`

`This mod uses a file watcher. If the configuration file is not changed with BepInEx Configuration manager, but changed in the file directly on the server, upon file save, it will sync the changes to all clients.`

### Compatible with:

* VNEI
* Jewelcrafting (never worry about losing your gems again!)
* EpicLoot (never worry about losing your enchanted items again!)
* AzuExtendedPlayerInventory
* Auga

### Localization

Recycle_N_Reclaim (RNR) supports localization. This means that you can create language files for different languages.
For example, to add a Swedish translation to this mod, a user could create a `Recycle_N_Reclaim.Swedish.yml` file inside
of
the config folder and add Swedish translations there.

* The following languages in addition to English are translated for you already but might not be fully accurate:
    * Russian
    * Chinese
    * French
    * German
    * Japanese
    * Korean
    * Spanish

---

## Original Author's Credits

All original code for the crafting tab/button was written
by [ABearCodes](https://valheim.thunderstore.io/package/abearcodes/SimpleRecycling/)   
Original Mod Link: [Simple Recycling](https://valheim.thunderstore.io/package/abearcodes/SimpleRecycling/)

## Mod Information

This mod is a combination
of [OdinsInventoryDiscard](https://valheim.thunderstore.io/package/OdinPlus/OdinsInventoryDiscard/) and the mod above.
The aim is to provide an all-in-one solution for
recycling items back into resources.

All code changes after the initial release of this mod was written by me. This includes the merging of the two mods,
addition of ServerSync and
any improvements made to the code.

<details>
<summary><b>Installation Instructions</b></summary>

***You must have BepInEx installed correctly! I can not stress this enough.***

### Manual Installation

`Note: (Manual installation is likely how you have to do this on a server, make sure BepInEx is installed on the server correctly)`

1. **Download the latest release of BepInEx.**
2. **Extract the contents of the zip file to your game's root folder.**
3. **Download the latest release of Recycle_N_Reclaim from Thunderstore.io.**
4. **Extract the contents of the zip file to the `BepInEx/plugins` folder.**
5. **Launch the game.**

### Installation through r2modman or Thunderstore Mod Manager

1. **Install [r2modman](https://valheim.thunderstore.io/package/ebkr/r2modman/)
   or [Thunderstore Mod Manager](https://www.overwolf.com/app/Thunderstore-Thunderstore_Mod_Manager).**

   > For r2modman, you can also install it through the Thunderstore site.
   ![](https://i.imgur.com/s4X4rEs.png "r2modman Download")

   > For Thunderstore Mod Manager, you can also install it through the Overwolf app store
   ![](https://i.imgur.com/HQLZFp4.png "Thunderstore Mod Manager Download")
2. **Open the Mod Manager and search for "Recycle_N_Reclaim" under the Online
   tab. `Note: You can also search for "Azumatt" to find all my mods.`**

   `The image below shows VikingShip as an example, but it was easier to reuse the image.`

   ![](https://i.imgur.com/5CR5XKu.png)

3. **Click the Download button to install the mod.**
4. **Launch the game.**

</details>

<br>
<br>

<details><summary><b>Configuration Options</b> (Azumatt.Recycle_N_Reclaim.cfg)</summary>

### Please note that Inventory Recycle and Reclaiming are different sections as well as different functionality within the game. Recycling happens only in the inventory and (by default) limited to admins only. Change the config should you wish to give this ability to everyone. Admins will always (by default) get 100% of the resources returned to them. Reclaiming happens in the crafting menu and is available to everyone. The amount of resources returned is configurable but is 50% by default.

#### What this looks like in the [BepInEx Configuration Manager](https://valheim.thunderstore.io/package/Azumatt/Official_BepInEx_ConfigurationManager/)

![image](https://github.com/AzumattDev/Recycle_N_Reclaim/assets/80414405/00f139cf-30a5-4433-b154-4c544aa1efd9)

`1 - General`

Lock Configuration [Synced with Server]

* If on, the configuration is locked and can be changed by server admins only.
    * Default Value: On

`2 - Inventory Recycle`

Enabled [Synced with Server]

* If on, you'll be able to discard things inside of the player inventory.
    * Default Value: On

Lock to Admin [Synced with Server]

* If on, only admin's can use this feature.
    * Default Value: On

DiscardHotkey(s) [Not Synced with Server]

* The hotkey to discard an item or regain resources. Must be enabled
    * Default Value: Delete

ReturnUnknownResources [Synced with Server]

* If on, discarding an item in the inventory will return resources if recipe is unknown
    * Default Value: Off

ReturnEnchantedResources [Synced with Server]

* If on and Epic Loot or Jewelcrafting is installed, discarding an item in the inventory will return resources for Epic
  Loot enchantments or Jewelcrafting gems
    * Default Value: On

ReturnResources [Synced with Server]

* Fraction of resources to return (0.0 - 1.0). This setting is forced to be between 0 and 1. Any higher or lower values
  will be set to 0 or 1 respectively.
    * Default Value: 1

`3 - Reclaiming`

RecyclingRate [Synced with Server]

* Rate at which the resources are recycled. Value must be between 0 and 1.
  The mod always rolls *down*, so if you were supposed to get 2.5 items, you would only receive 2. If the recycling rate
  is 0.5 (50%), the player will receive half of the resources they would usually need to craft the item, assuming a
  single item in a stack and the item is of quality level 1. If the item is of higher quality, the resulting yield would
  be higher as well.
    * Default Value: 0.5

ReturnEnchantedResources [Synced with Server]

* If on and Epic Loot or Jewelcrafting is installed, discarding an item in the inventory will return resources for Epic
  Loot enchantments or Jewelcrafting gems
    * Default Value: On

UnstackableItemsAlwaysReturnAtLeastOneResource [Synced with Server]

* If enabled and recycling a specific _unstackable_ item would yield 0 of a material,
  instead you will receive 1. If disabled, you get nothing.
    * Default Value: On

RequireExactCraftingStationForRecycling [Synced with Server]

* If enabled, recycling will also check for the required crafting station type and level.
  If disabled, will ignore all crafting station requirements altogether.
  Enabled by default, to keep things close to how Valheim operates.
    * Default Value: On

PreventZeroResourceYields [Synced with Server]

* If enabled and recycling an item that would yield 0 of any material,
  instead you will receive 1. If disabled, you get nothing.
    * Default Value: On

AllowRecyclingUnknownRecipes [Synced with Server]

* If enabled, it will allow you to recycle items that you do not know the recipe for yet.
  Disabled by default as this can be cheaty, but sometimes required due to people losing progress.
    * Default Value: Off

`4 - UI`

ContainerButtonPosition [Synced with Server]

* The last saved recycling button position stored in JSON
    * Default Value: {"x":496.0,"y":-374.0,"z":-1.0}

ContainerRecyclingEnabled [Synced with Server]

* If enabled, the mod will display the container recycling button
    * Default Value: On

NotifyOnSalvagingImpediments [Synced with Server]

* If enabled and recycling a specific item runs into any issues, the mod will print a message
  in the center of the screen (native Valheim notification). At the time of implementation,
  this happens in the following cases:

- not enough free slots in the inventory to place the resulting resources
- player does not know the recipe for the item
- if enabled, cases when `PreventZeroResourceYields` kicks in and prevent the crafting
    * Default Value: On

EnableExperimentalCraftingTabUI [Synced with Server]

* If enabled, will display the experimental work in progress crafting tab UI
  Enabled by default.
    * Default Value: On

HideRecipesForEquippedItems [Synced with Server]

* If enabled, it will hide equipped items in the crafting tab.
  This does not make the item recyclable and only influences whether or not it's shown.
  Enabled by default.
    * Default Value: On

IgnoreItemsOnHotbar [Synced with Server]

* If enabled, it will hide hotbar items in the crafting tab.
  Enabled by default.
    * Default Value: On

StationFilterEnabled [Synced with Server]

* If enabled, will filter all recycling recipes based on the crafting station
  used to produce said item. Main purpose of this is to prevent showing food
  as a recyclable item, but can be extended further if needed.
  Enabled by default
    * Default Value: On

StationFilterList [Synced with Server]

* Comma separated list of crafting stations (by their "prefab name")
  recipes from which should be ignored in regards to recycling.
  Main purpose of this is to prevent showing food as a recyclable item,
  but can be extended further if needed.

Full list of stations used in recipes as of 0.216.9:

- identifier: `forge` in game name: Forge
- identifier: `blackforge` in game name: Black Forge
- identifier: `piece_workbench` in game name: Workbench
- identifier: `piece_cauldron` in game name: Cauldron
- identifier: `piece_stonecutter` in game name: Stonecutter
- identifier: `piece_artisanstation` in game name: Artisan table
- identifier: `piece_magetable` in game name: Galdr table

    * Default Value: piece_cauldron

`zDebug`

DebugAlwaysDumpAnalysisContext [Synced with Server]

* If enabled will dump a complete detailed recycling report every time. This is taxing in terms
  of performance and should only be used when debugging issues.
    * Default Value: Off

DebugAllowSpammyLogs [Synced with Server]

* If enabled, will spam recycling checks to the console.
  VERY. VERY. SPAMMY. Influences performance.
    * Default Value: Off

</details>

<br>

<details><summary><b>Example YAML</b> (Azumatt.Recycle_N_Reclaim_ExcludeLists.yml)</summary>

```yaml
# Below you can find example groups. Groups are used to exclude or includeOverride quickly. They are reusable lists! 
# Please note that some of these groups & limitations are kinda pointless but are here for example.
# Make sure to follow the format of the example below. If you have any questions, please ask in my discord.

# Full vanilla prefab name list: https://valheim-modding.github.io/Jotunn/data/prefabs/prefab-list.html
# Item prefab name list: https://valheim-modding.github.io/Jotunn/data/objects/item-list.html

# There are several predefined groups set up for you that are not listed. You can use these just like you would any group you create yourself.
# These are the "All", "Food", "Potion", "Fish", "Swords", "Bows", "Crossbows", "Axes", "Clubs", "Knives", "Pickaxes", "Polearms", "Spears", "Equipment", 
#  "Boss Trophy", "Trophy", "Crops", "Seeds", "Ores", "Metals", "Woods", "Armor", "Helmets", "Ammunition", "Utilities", "Tools", "Miscellaneous", and "Customizations" groups.
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
#     - itemType: Trophie
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
#   Armor:
#     - itemType: Chest, Shoulder, Legs, Hands
#   Helmets:
#     - itemType: Helmet
#   Ammunition:
#     - itemType: Ammo, AmmoNonEquipable
#   Utilities:
#     - itemType: Utility
#   Tools:
#     - itemType: Tool
#   Miscellaneous:
#     - itemType: Misc
#   Customizations:
#     - itemType: Customization
#   All:
#     - Criteria: Item has an ItemDrop script and all needed fields are populated. (all items)




groups:
  Example Group: # Group name
    - APrefabName # Item prefab name, note that this is case sensitive and must be the prefab name
  Another Custom Group: # Group name
    - APrefabName # Item prefab name, note that this is case sensitive and must be the prefab name
    - AnotherPrefabName
    - YetAnotherPrefabName
  Tier 2 Items: # Group name
    - Bronze # Item prefab name, note that this is case sensitive and must be the prefab name
    - PickaxeBronze
    - ArmorBronzeChest
    - ArmorBronzeLeggings


# Inventory section determines which items can be recycled. Remember that recycling from inventory is defaulted to only admins.
inventory:
  exclude: # Exclude these items from being recycled
    - Metals # Exclude all items in the "Metals" group from being recycled in inventory
  includeOverride:
    - Metals # Override the setting above, allowing "Metals" group to be recycled in inventory

# Reclaiming section determines which items can be reclaimed via Containers or the Reclaim tab.
reclaiming:
  exclude:
    - Metals # Exclude all items in the "Metals" group from being reclaimed
    - Armor # Exclude all items in the "Armor" group from being reclaimed
    - Helmets # Exclude all items in the "Helmets" group from being reclaimed
    - Hammer # Exclude this specific item from being reclaimed
  includeOverride:
    - All # Allow all items to be reclaimed, overrides the exclude rules above for "reclaiming" section

# Containers section determines the rules for specific containers. It follows the limitations of the "reclaiming" section to determine what is actually reclaimed.
# This section is primarily used for managing the items included or excluded from the "Reclaim All" functionality of containers, allowing you to prevent certain items 
# from being a part of the reclaim logic.
containers:
  piece_chest: # Container prefab name, note that this is case sensitive and must be the prefab name
    exclude:
      - Food # Exclude or "skip" all items in the "Food" group from this container. Food will not be deconstructed back into its ingredients.
      - PickaxeBronze #  Exclude or "skip" this specific item from this container. Excluding it from being reclaimed will prevent it from being deconstructed back into its ingredients.
    includeOverride:
      - Foods # Override
      - PickaxeBronze # Allow this specific item to be included in the reclaiming process. Overrides the exclude rules above.
      - All # Just here for cleaning up the example, allowing default behavior

  piece_chest_wood:
    exclude:
      - Swords # Exclude all items in the "Swords" group from this container
      - Tier 2 Items # Exclude all items in the "Tier 2 Items" group from this container
      - Bows # Exclude all items in the "Bows" group from this container
    includeOverride:
      - BowFineWood # Allow this specific item to be included in this container
      - Wood # Allow this specific item to be included in this container
      - Bronze # Allow this specific item to be included in this container
      - All # Just here for cleaning up the example, allowing default behavior

  piece_chest_private:
    exclude:
      - All # Exclude all items from this container
    includeOverride:
      - All # Just here for cleaning up the example, allowing default behavior

  piece_chest_blackmetal:
    exclude:
      - Swords # Exclude all items in the "Swords" group from this container
      - Tier 2 Items # Exclude all items in the "Tier 2 Items" group from this container
      - Bows # Exclude all items in the "Bows" group from this container
    includeOverride:
      - BowFineWood # Allow this specific item to be included in this container
      - Wood
      - Bronze
      - All # Just here for cleaning up the example, allowing default behavior
```

</details>

<br>

<p align="center">
  <img alt="2023-06-22_11-33-22" src="https://github.com/AzumattDev/SkillManagerModTemplate/assets/80414405/2dbbe853-eccc-460c-bf41-111f38d0a6ac"/>
</p>
<img src="https://github.com/AzumattDev/Recycle_N_Reclaim/assets/80414405/cd4e10be-1728-435a-ae3f-47b7daa2f3cd" alt="E1CB4F06-72CE-43BC-9FFC-1E53E89640EE-min" width="100%" style="max-width: 1280px; height: auto;">

<img src="https://github.com/AzumattDev/Recycle_N_Reclaim/assets/80414405/102410f4-4b8a-4cd4-919e-421ddb33db38" alt="5B0B26B8-8064-421E-8888-6D40E71C56DC-min" width="100%" style="max-width: 1280px; height: auto;">
<img src="https://github.com/AzumattDev/Recycle_N_Reclaim/assets/80414405/385e58d7-96d2-4546-8577-d612d804e194" alt="5B0B26B8-8064-421E-8888-6D40E71C56DC-min" width="100%" style="max-width: 1280px; height: auto;">
<img src="https://github.com/AzumattDev/Recycle_N_Reclaim/assets/80414405/838b9ddd-9105-4478-9bf1-0b6c9859b4b5" alt="5B0B26B8-8064-421E-8888-6D40E71C56DC-min" width="100%" style="max-width: 1280px; height: auto;">


`Feel free to reach out to me on discord if you need manual download assistance.`

# Author Information

### Azumatt

`DISCORD:` Azumatt#2625

`STEAM:` https://steamcommunity.com/id/azumatt/

For Questions or Comments, find me in the Odin Plus Team Discord or in mine:

[![https://i.imgur.com/XXP6HCU.png](https://i.imgur.com/XXP6HCU.png)](https://discord.gg/Pb6bVMnFb2)
<a href="https://discord.gg/pdHgy6Bsng"><img src="https://i.imgur.com/Xlcbmm9.png" href="https://discord.gg/pdHgy6Bsng" width="175" height="175"></a>