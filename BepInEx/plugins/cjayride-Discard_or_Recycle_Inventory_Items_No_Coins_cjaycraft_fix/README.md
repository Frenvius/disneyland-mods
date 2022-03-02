This is a fork from the original mod: Discard or Recycle Inventory Items 
https://www.nexusmods.com/valheim/mods/45

The mod has now developed and changed into something far different from the original.

## WARNING: Players using Better Archery and More Slots
This mod is compatible, but you must read and follow all steps for proper configuration!

## This mod recycles items into parts

- Break down (recycle) items on the fly, by drag clicking an item and clicking [Delete]

- Control the percentage (%) of parts returned (in the config)

- Control the types of parts to be recycled (enchantment parts, coins, consumables)

## Setup
There are important configuration settings if you use one of the following mods.
- Better Archery
- More Slots (or another mod that adds rows to your inventory)

## "Better Archery" Mod Players

The following configuration makes this mod compatible with Better Archery

> // Set to 'true' if you're using the Better Archery mod

> // Setting type: Boolean

> // Default value: false

**UsingBetterArchery = true**

> // Developer information: Better Archery adds 16 item slots to your total inventory, and counts the 3 quiver slots as regular inventory slots, even though it can only hold arrows.

## Better Archery + "Extra Slots" Mod Players

The following configuration makes this mod compatible with Better Archery and More Slots

The number of inventory rows you're playing with will affect calculations. Default is 4. Some mods add more rows, **so you need to change this here for the mod to work with BetterArchery**. If you're not using BetterArchery, this value doesn't matter because the code will never be reached. 

> // Default value: 4

InventoryRows = 4

> // Developer information: BetterArchery quiver slots are 2 rows below your last inventory row.


## Recycle EpicLoot Enchanted Gear for Magic Parts

> // Return resources for Epic Loot enchantments

> // Setting type: Boolean

> // Default value: true

**ReturnEnchantedResources = true**

## Don't Give Players Coins

When recycling parts, don't give Coins (enable/disable).

It cost Coins to enchant with Epic Loot, so if you recycle an item it will usually return Coins. Some servers and players may not want this. Items gave back too many coins and it messed up our server economy.

> // Enable/disable coins on recycling items

> // Setting type: Boolean

> // Default value: false

**RecycleCoins = false**

## Don't Recycle Consumables

Don't allow recycling items that have consumables as parts (enable/disable).

On our server, we didn't want people recycling food because it gave certain items that might affect the economy.

By default, this mod will allow you to recycle consumables unless turned off. 

> // Enable/disable recycling of consumables (like food)

> // Setting type: Boolean

> // Default value: true

**RecycleConsumables = true**

## Edit the config file
> **BepInEx/config/aedenthorn.DiscardInventoryItemCJAYCRAFT-fix.cfg**

Launch the game once to generate the config file and review the options.

If you installed a version before 1.3.2 -- make sure re-generate the config file to get all of the new options.

**RecycleTrophy = true**

## Edit the config file
> **BepInEx/config/aedenthorn.DiscardInventoryItemCJAYCRAFT-fix.cfg**

If false, you won't be able to recycle items that give back trophies. This needs to be set to false for the cjaycraft_ultimate_modpack to work because of the enchanting/rune/magic recipes.

## Change log

**1.3.3** - 2022/2/28

- Added a configuration option to enable or disable materials that give back Trophys (Trophies). RecycleTrophy = false needs to be set in order for the cjaycraft_ultimate_modpack to work, because of the enchanting/rune recipes.


**1.3.2** - 2022/2/16

- Fixed bug where RecycleCoins = true -- would previously not give back any coins. Default setting is RecycleCoins = false

**1.2.1** - 2022/2/9

- Added a configuration option to enable or disable the recycling of consumables (like food).

**1.2.0**

 - Fixed a bug that still existed when **Better Archery** was installed because it messes up the available inventory slot calculations. I really hope this is the last fix after spending many hours trial and error. Thank you for your patience this has been really tough. Thank you to mod tester Moniker.

*Programmer Details: Better Archery always add an additional 16 item slots to your inventory (invisible). The 3 quiver slots are always 2 rows below your last inventory row.*

- Fixed a bug when **More Slots** or other inventory row adding mod is installed **with Better Archery at the same time.**

Programmer Details: The "More Slots" rows expands your inventory, and then Better Archery quiver slots are added on a different inventory row from default, and we need to account for this.

**1.1.0**

- Fixed bug where items only recycle if **BetterArchery** is installed.

- Added new config options:

  `UsingBetterArchery = false`

  `BetterArcheryInventoryCount = 16`
  (don't change this unless you absolutely know what

  If using Better Archery mod, set **UsingBetterArchery = True** (false by default)

  Leave **BetterArcheryInventoryCount = 16** alone unless you absolutely know what you're doing. Better Archery seems to add 16 invisible slots, so this is a fix workaround.
  
- Fixed bug where if the empty slots are your first row of inventory, and the rest of your inventory is full, the recycled Items won't be added and are lost. Added error checking so that the empty slots need to be below your first row in the bag in order to recycle.

1.0.4 - fix text formatting in README.md - no mod update

1.0.3 - updated README.md and icon.png - no mod update

1.0.2 - original upload with no known issues

## GitHub

This mod: https://github.com/cjayride/ValheimMods/tree/master/DiscardInventoryItem

Original Mod: https://github.com/aedenthorn/ValheimMods/tree/master/DiscardInventoryItem

## Contact

Twitter: twitter.com/cjayride

Discord: discord.gg/cjayride (find me at the top of the user list) "cjayride"

## Livestreams

IRL: twitch.tv/cjayride

Gaming: twitch.tv/cjaywalk