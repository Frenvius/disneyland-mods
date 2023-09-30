![#JötunnBackpacks](https://live.staticflickr.com/65535/51349781473_97b6d4ae9d_h.jpg)

This mod introduces two backpack models (thanks to Cinnabunn!) to the game. You can open them with a hotkey (_i_ by default) and store items in them. It's an expansion on Aedenthorn's [BackpackRedux](https://www.nexusmods.com/valheim/mods/1333) mod, and it relies heavily on their precursor work.

### Features
* Each backpack has its own separate inventory, and their inventories are preserved even when you toss your backpack to a friend.
* Storing items in the backpack reduces their weight by 50% by default (configurable).
* You can also configure how much they modify your carry capacity and movement speed.
* [Localization support](https://valheim-modding.github.io/Jotunn/tutorials/localization.html#example-json-file). Please let me know if you want to add a translation for your language!
* You cannot teleport with unteleportable items in the backpack.
* Nor can you put a backpack inside a backpack in order to get around this limitation!

### Server
* Should be installed on both server and on all clients. If the mod is on the server, it will disconnect clients without the mod.
* All configs (except hotkey) are server-enforceable.

### Credits
Feel free to show appreciation by supporting. :)

 * **Cinnabunn** (_support_) for their amazing art.
 * **Aedenthorn** ([support](https://www.nexusmods.com/valheim/users/18901754)).
 * **Randy Knapp** ([support](https://www.paypal.com/donate/?hosted_button_id=UFYR7AKYFPXLY)) for their [Extended Item Data Framework](https://github.com/RandyKnapp/ValheimMods/tree/main/ExtendedItemDataFramework). Also this [fix](https://github.com/RandyKnapp/ValheimMods/blob/77e98e3cf0cacc43d9812659f12fd5fcb3154d8d/EquipmentAndQuickSlots/InventoryGrid_Patch.cs#L10).
 * **paddywaan** for fixing some of my code and adding a feature [via PR](https://github.com/Emrik-North/JotunnBackpacks/commit/335c3b7253eb5c8621b812cb19c858e5bf03234d).
 * **Zarboz** for guidance and [help](https://github.com/VMP-Valheim/Back_packs) with the implementation.
 * **The Jotunn Team** for creating [Jotunn: The Valheim Library](https://valheim-modding.github.io/Jotunn/index.html).
 * **MarcoPogo** and **Jules** for helping me with some questions I had in the [Jotunn Discord](https://discord.gg/DdUt6g7gyA).

Most of this project is the result of the hard work of these awesome people!

### Compatibility Notes
 * Compatible with _[Project Auga](https://projectauga.com/)!_
 * Minor compatibility [issue](https://forums.nexusmods.com/index.php?/topic/10327288-jotunnbackpacks/page-6#entry98033203) with _Backpack Redux_.

Please let me know if you find any additional bugs, issues or incompatibilities.

### How to Install
0. _(Optional)_ Use a mod manager like [r2modman](https://valheim.thunderstore.io/package/ebkr/r2modman/) or alternatives.
1. Install [BepInEx for Valheim](https://valheim.thunderstore.io/package/denikson/BepInExPack_Valheim/).
2. Install [Jotunn](https://valheim.thunderstore.io/package/ValheimModding/Jotunn/).
3. Install [Extended Item Data Framework](https://valheim.thunderstore.io/package/RandyKnapp/ExtendedItemDataFramework/).
4. Install this mod.

For manual install, you want to drag the _JotunnBackpacks_ folder into the BepInEx/Plugins folder. The _JotunnBackpacks_ folder should contain _JotunnBackpacks.dll_ and _Translations_.

### Changelog
**2.0.0**
 * Added Quickdrop feature like in Outward!
 * Made the size configuration separate for the two backpacks ([paddywaan](https://github.com/paddywaan/) contribution!)
 * Added Russian translation (thanks [to](https://github.com/Emrik-North/JotunnBackpacks/issues/2) Dominowood371 and Mi4oko!)
 * Dropping items directly from backpack inventory now updates player inventory weight ([bug report](https://www.nexusmods.com/valheim/mods/1416?tab=bugs))
 * Unequipping or dropping worn backpack now closes its inventory if it was open ([bug report](https://www.nexusmods.com/valheim/mods/1416?tab=bugs))
 * Cold/freezing protection is now configurable ([feature request](https://github.com/Emrik-North/JotunnBackpacks/issues/3))
 * Rugged backpack now costs 2 bronze, so it's accessible early game.

### Links
[Thunderstore](https://valheim.thunderstore.io/package/EmrikNorth_and_Aedenthorn/JotunnBackpacks/)  
[Nexusmods](https://www.nexusmods.com/valheim/mods/1416)  
[GitHub](https://github.com/Emrik-North/JotunnBackpacks)  
