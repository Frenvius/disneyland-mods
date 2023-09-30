# Add All Fuel And Ore For Smelter Charcoal kiln etc

## Features

* You no longer need to press the button repeatedly to get to the furnace.
* When using the facility normally (default: E), fuel is fed one by one.
* When using the facility, pressing the modifier key (default: Left Shift) will load the fuel, etc. in batches.

## Description

* If there is no fuel in the player's inventory, fuel can be injected in batches from containers.
* If you want to use this feature, you need to change the settings.

* If a player's inventory and containers do not reveal a valid item when in individual item mode (default E), the other mods will continue to process the item.
* Note that in batch mode (default: Shift Left + E), other mods will not continue to process if an item is not found.

* The unit of batch injection is done per stack.
  * For example, if you have wood (10/50) and wood (20/50) in your inventory, 10 of them will be consumed from your inventory.
  * If you do it again, 20 of them will be consumed.
  * If the fuel limit is less than the stack, only that amount will be consumed.

## Conflict

## Setting

* The configuration file is "BepInEx/config/rin_jugatla.AddAllFuel.cfg".It will be created automatically when you start the game after installing the mod.

1. Enabled
   * true: MOD enabled
   * false: Mod disabled
2. NexusID
   * ID for automatic update notification, no need to change.
3. ModifierKey
   * Modifier key used to control batch injection.
4. IsReverseModifierMode
   * true: use key (E) for batch input
   * false: use modifier key (left shift) + use key (E)
5. ExcludeNames
   * Item name to exclude from submission.
   * Example: $item_finewood,$item_roundlog
   * Refer to this document for item names.
6. AllowAddOneExcludeItem
   * true: Exclude items from the list if they are submitted individually.
   * false: Do not allow items to be submitted regardless of whether they are submitted individually or in batches
7. UseFromContainer
   * true: If there is no fuel in the player's inventory, it will be replenished from a nearby container.
   * false: We will not replenish from the container.
8. UseFromContainerRange
   * The distance from the player to the container when refilling from the container.

## Supported Facilities

1. Smelter
2. Charcoal kiln
3. Blast furnace
4. Windmill
5. Spinning wheel
6. Campfire
7. Various torches

## Changelog

### Comfy Version Update

### 1.7.0

  * Added compatibility for mistlands by updating GetItem(string) to GetItem(string, int, bool)
  * Added compatibility for mistalnds by updating Smelter.OnAddFuel and Smelter.OnAddore signatures

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
