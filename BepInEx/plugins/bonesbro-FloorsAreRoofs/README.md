# Details for Real People
Are you a simple man, with simple needs for entirely box-like buildings?  Do you feel oppressed and stifled having to build angled roofs like some sort of... person?  Well, take heart, brave viking: there's a mod for that.

This mod edits wooden floors so that they are considered roofs, allowing you to build and use a bed or workbench underneath them.  You gain rested bonuses and comfort and all of the usual stuff.  They are also updated so that they do not take damage and decay in the rain and will shield the pieces below them from rain damage.

Let's be honest... building this way can be kind of ugly.  But for some purposes, like a tower or a rooftop deck, it'll be helpful AND aesthetic.  Use your new power wisely.

# Installation
Extract the .dll file to your Valheim\BepInEx\plugins\ folder, just like you do with every other mod.

Supports Nexus Update Check﻿ if it is installed.  It is not required.

# Technical Words for Nerds
Valheim considers the player sheltered if two things are true:
The area above the player is covered with a surface that does not have the "leaky" tag.
If you draw a line out in every direction from the player, most of them run into a structure or terrain.

This mod affects calculation #1 by finding the wood_floor and wood_floor1x1 pieces and updating the tag on their colliders from "leaky" to "roof", matching the tag used on pieces like wood_roof.  This should be a safe operation with little chance for side effects.  The "leaky" tag is only used for the "is roofed" check used by beds, crafting stations, and rain damage calculations, and the "roof" tag is not currently used at all.

There's detailed logging written to your Player.log file.  Search for "floorsareroofs".

# Support for Custom Pieces
Version 2.0 allows you to control which pieces are updated by editing the config file, which is automatically generated into BepInEx/config/bonesbro.val.floorsareroofs.cfg after you've launched the game with the mod once.

Sample config entries to add support for the wooden floor pieces added by Odin's Architect:

> \## List of the prefab pieces to weatherproof.  Comma-separate each prefab name.  Default: wood_floor,wood_floor_1x1
>
> PrefabsToChange = wood_floor,wood_floor_1x1,IG_Chevron_Floor,IG_Hardwood_Floor,IG_Big_Chevron_Floor,IG_Big_Hardwood_Floor

> \## List of hammer tools whose recipes we'll search to find the pieces to update.  These are the prefab names for each hammer piece.  Comma-separate each prefab name.  Default: Hammer
> 
> Hammers = Hammer,odin_hammer


If you don't need custom pieces then you don't need to do anything; by default it will only modify only the vanilla pieces.  If you're loathe to install Jotunn (a common library used by many mods) then you can use the older version 1.1.  Version 1.1 still works with Mistlands.

# Source Code
https://github.com/bonesbro/ValFloorsAreRoofs

# Changelog
2.0.1: No code change, just fixed the dependencies to add Jotunn.
2.0.2: Add Jotunn as a BepInDependency to ensure that loading happens in the right order.
