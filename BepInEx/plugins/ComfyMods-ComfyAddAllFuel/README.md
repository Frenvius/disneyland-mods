# Comfy Add All Fuel

## Features

* You no longer need to press the button repeatedly to add fuel, food, ore, etc.
* When using the any smelters, cooking stations, or fireplaces, interact key (default e) will behavior as normal
* When pressing the modifier key, batch adding will be attempted up to the fuel/food/ore limit.

## Description

* The unit of batch injection is done per stack.
  * For example, if you have wood (10/50) and wood (20/50) in your inventory, 10 of them will be consumed from your inventory.
  * If you do it again, 20 of them will be consumed.
  * If the fuel limit is less than the stack, only that amount will be consumed.

## Settings

1. Enabled
   * true: MOD enabled
   * false: Mod disabled
2. ModifierKey
   * Modifier key used to control batch injection.
3. ExcludeNames
   * Item name to exclude from submission.
   * Example: $item_finewood,$item_roundlog
   * Refer to this document for item names.

## Supported Consumers

1. Smelter
2. Charcoal kiln
3. Blast furnace
4. Windmill
5. Spinning wheel
6. Campfire
7. Ovens
8. Cooking Stations
9. Various torches

## Changelog

### Comfy Version Update

### 1.8.1

  * Fixed bug where incorrect number of items removed from inventory.

### 1.8.0

  * Added support for cooking stations
    * Ovens: fuel and food
    * Cooking station: food
    * Iron cooking station: food
  * Remove all items from cooking station by holding modifier key (provided all slots are full)
  * Updated references to valheim_data\Managed from unstripped_corlib
  * Refactored
  * Updated readme

### 1.7.2

  * Removed all logging

### 1.7.1

  * Removed unnecessary logging statements.

### 1.7.0

  * Added compatibility for mistlands by updating GetItem(string) to GetItem(string, int, bool)
  * Added compatibility for mistlands by updating Smelter.OnAddFuel and Smelter.OnAddore signatures
  * Refactor patches into patch folder and respective Object.cs files

### 1.6.3

* Removed ability to get items from nearby chests and retains only ability to batch add fuel and ore.

### 1.6.2

* There was an error in the changelog for version 1.6.1, which has been corrected.
* There is no change in the program content.

* Fixed a bug that caused items to be lost in version 1.6.0.
* We believe that this bug was caused by the server not being able to send the correct commands when batch-loading items.
* As a result of this fix, the effects of batch item submissions are now displayed multiple times.
* If you are using version 1.6.0, please update to version 1.6.1 or 1.6.2 .

### 1.6.1

* This version may have a bug that causes items to be lost.
* Rewind the effect processing when fueling, which was changed in version 1.6.0.
* This may have caused items to be lost due to a lack of coordination with the server.

### 1.6.0

* Changed so that the effect is only displayed once when items are inserted in bulk.
* Fixed a bug that caused an error when no storage is found nearby.

### 1.5.1

* Fixed a conflict with the "Craft Build Smelt Cook Fuel From Containers" mod!
* If a player's inventory and containers do not reveal a valid item when in individual item mode (default E), the other mods will continue to process the item.
* Note that in batch mode (default: Shift Left + E), other mods will not continue to process if an item is not found.

### 1.5.0

* Batch loading of fuel from containers is now supported.

### 1.4.0

* Batch feeding to campfire and torch is now supported.

### 1.3.0

* Added an option to exclude items used to input fuel, etc.
* Added option to throw in even excluded items when throwing in fuel, etc. one at a time.
* The ability to refill items from containers in the "Craft Build Smelt Cook Fuel From Containers" mod has been disabled, except for the input of charcoal.

### 1.2.1

* Fixed a bug that caused items to be duplicated when used in conjunction with the "Craft Build Smelt Cook Fuel From Containers" mod.

### 1.2.0

* Added an option to change the switching between feeding items one at a time or in batches.
* Change "IsReverseModifierMode" in the configuration file (rin_jugatla.AddAllFuel.cfg).
* false: Batch submit with Modifier key (left shift) + Use key (E)
* true: Use key (E) to submit all

### 1.1.0

* Changed to use the mod when using the facility while holding down the modifier key (default: left shift).
* Added support for NexusUpdateMOD.
