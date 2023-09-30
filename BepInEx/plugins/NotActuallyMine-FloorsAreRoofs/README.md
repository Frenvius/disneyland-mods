**Ported from the Nexus Mods, I do not maintain this mod but will update it if a new version is uploaded on Nexus (If I remember), I cannot add features.** 

This was uploaded so some friends who don't know how to manually download and install mods from Nexus can use it, I hope it helps you as well.

## Details for Real People

Are you a simple man, with simple needs for entirely box-like buildings?  Do you feel oppressed and stifled having to build angled roofs like some sort of... person?  Well, take heart, brave Viking: there's a mod for that.

This mod edits wooden floors so that they are considered roofs, allowing you to build and use a bed or workbench underneath them.  You gain rested bonuses and comfort and all of the usual stuff.  They are also updated so that they do not take damage and decay in the rain and will shield the pieces below them from rain damage.

Let's be honest... building this way can be kind of ugly.  But for some purposes, like a tower or a rooftop deck, it'll be helpful AND aesthetic.  Use your new power wisely.

## Installation

Either use the Thunderstore Mod Manager or extract the .dll file to your Valheim\BepInEx\plugins\ folder, just like you do with every other mod.

Doesn't support Nexus Update Check, because this is on Thunderstore, that isn't Vortex nor Nexus.  It is not required, and can't be used, because this is Thunderstore.

## Technical Words for Nerds

Valheim considers the player sheltered if two things are true:
The area above the player is covered with a surface that does not have the "leaky" tag.
If you draw a line out in every direction from the player, most of them run into a structure or terrain.

This mod affects calculation #1 by finding the wood_floor and wood_floor1x1 pieces, finds their colliders, and changes the collider's tag from "leaky" to "roof", matching the tag used on pieces like wood_roof.  The "leaky" tag is only used for the "is roofed" check used by beds, crafting stations, and rain damage calculations. The "roof" tag is not currently used at all.