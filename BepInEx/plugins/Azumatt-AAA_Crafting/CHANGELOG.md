> # Update Information (Latest listed first)
> ### v1.3.2
> - Update internal AugaAPI and JewelcraftingAPI
> - Search box can now search by mod name. Do @modname to search for items from that mod. Example: @jewelcrafting will return all items from Jewelcrafting.
> ### v1.3.1
> - Auga's update broke compatibility already. I fixed that yet again.
> - Note: The UI is still a bit wonky with Auga for various reasons. I'll fix that later with Vapok. It's not game breaking, just annoying.
> - Also note: Full functionality of this mod is now available with Auga installed.
> ### v1.3.0
> - Update ServerSync.dll
> - Compile against 0.217.28
> - PARTIAL Auga support. Pushing code early for Valheim's update. I'll finish it up later. Should work okay, but makes the multicrafting part of this not work right yet due to how they do the crafting button.
> ### v1.2.1
> - You can now prefix your searches with an ! to search for recipe requirements. Example: !refined will return all items that require refined eitr. Please note: It's a contains on the string and will also return anything with that in the name. So !wood will return wood, fine wood, core wood, etc.
> ### v1.2.0
> - Add ServerSync. Crafting time is now synced with the server by default. All other configs are not as they don't affect gameplay. Added this by request. I personally didn't mind this being client only config. :D
> - Fix an issue you might encounter with Jewelcrafting mod installed. Where, if a item breaks during socketing and the recipe changes to another, it will now stop crafting.
> ### v1.1.1
> - Fix a small issue with the requirement text
> - Change where the search box is located and make it look more in line with the vanilla UI
> ### v1.1.0
> - Update for latest Valheim changes.
> ### v1.0.10
> - Update for Hildir's Request 0.217.14 (seems it just needed a recompile)
> ### v1.0.9
> - Generic updates as well as a small update for Valheim 0.216.9
> ### v1.0.8
> - Fix some errors that could happen if other mods were installed that didn't populate the crafting requirements correctly on their items.
> ### v1.0.7
> - Added in compatibility for OdinsCraftyBoxes and CraftFromContainers. The values should now show appropriately. Keep
    in mind Aedenthorn/Aedenthorn's collaborators have multiple versions of their mod. I have only provided
    compatibility with the one directly called CraftFromContainers, I am unsure if the other versions work.
> ### v1.0.6
> - Added a configuration option to change the requirement text format. Just in case that has been annoying you. (Default: {0} / {1})
    >   - {0} is the available amount the player has
>   - {1} is the requirement amount to make the item.
> ### v1.0.5
> - Fix bugs with the pagination/searching addition. Guess we fucked up eh? That's life.
> ### v1.0.4
> - Add in KG's pagination/searching addition. Thanks KG!
> ### v1.0.3
> - Added a configuration option to keep your crafting amount when switching recipes and after crafting completes.
> - Fix logging out and back in causing the UI not to rebuild
> - Fix the display affecting the build menu as well
> - Stop crafting if the active recipe changes
> ### v1.0.2
> - Keep your crafting amount when switching recipes or hitting the crafting button. (Just crafted 20 arrows? Switching
    to torches, hit craft, it will craft 20 torches as well until the value is changed.)
> ### v1.0.1
> - Moved to InventoryGui.Awake() to prevent issues with other mods.
> ### v1.0.0
> - Initial Release