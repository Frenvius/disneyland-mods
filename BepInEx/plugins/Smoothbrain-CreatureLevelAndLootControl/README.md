Adds various options to adjust combat difficulty and rewards.

Too lazy to read all these words below? Watch this short [introduction video](https://www.youtube.com/watch?v=UvJKPhC-zgM) by Timo_Redbeard instead.

## Feature overview
- Highly configurable, everything can be disabled and adjusted to your liking
- Creatures can spawn with up to 5 stars (no maximum for custom difficulty)
- Creatures that usually cannot level up can spawn stars as well
- Bosses can spawn with as many stars as you want to
- Increased size for creatures and bosses based on level
- Multiple ways to adjust the difficulty of the game
- Respawnable camps and dungeons
- Loot multipliers, even for bosses and trophies
- Affixes for bosses
- Special effects for creatures
- Adjustable damage and health gain per player for multiplayer games
- Adjustable range for creature nameplates to be displayed on mouseover
- Bonus level, if you kill a lot of creatures in a small area in a short time
- Can be installed on the server, to synchronize configuration in real time
- A public API that can be used by mod authors to make their mod interact with CLLC


## Creatures
Creature level can be adjusted in multiple ways:
You can set a difficulty that increases the level up chance of creatures or you can create your own difficulty.
As a second factor for difficulty, you can pick one of these options:
- Days passed in your world
- Distance from the initial spawning point
- Number of killed bosses in your world


Or you can disable the second factor, if you don't want to use it. Or you can just set a fixed level for all creatures or disable the level up for creatures completely.
Also, this mod enables leveling for creatures that usually cannot level up, like Serpents, Deathsquitos, Lox, Drakes, Wraiths, ...
You can even let camps and dungeons respawn!

## Creature star colors
Creatures can spawn with differently colored stars, if you want to. Each color tweaks the creature in a different way:

**Magenta** - Quick - Moves faster<br>
<small>40% increased movement speed</small>

**Red** - Aggressive - Attacks faster and tries to hit you more often<br>
<small>Attack speed increased by 25%, interval between two attack waves and circle time reduced by 50%, interval between circles increased by 150%</small>

**Green** - Regenerating - Regenerates health over time<br>
<small>BaseHeal = Health at 0 stars * (1 + 0.25 * stars), Healing = BaseHeal * (10 * log(max(10, BaseHeal - 1000)) / (BaseHeal + 1000)) * 1.2 / second</small>

**Cyan** - Curious - Comes checking for you from a farther distance<br>
<small>Hear and view range increased by 100%</small>

**White** - Splitting - Splits in two lower level enemies with the same color upon death<br>
<small>Example: A 4 star Greydwarf will split into two 2 star Greydwarfs on death</small>

**Blue** - Armored - Takes less damage, but moves slower<br>
<small>66% less damage taken, 50% reduced movement speed</small>

## Creature elemental infusions
Creatures can spawn with different elemental infusions, if you want to. Each infusion adds elemental effects to the creature:

**Fire-Infused** - Resistant to fire damage and vulnerable to frost damage. Ignites you on hit.<br>
**Frost-Infused** - Resistant to frost damage and vulnerable to fire damage. Freezes you on hit.<br>
**Lightning-Infused** - Resistant to lightning damage and vulnerable to spirit damage. Deals lightning damage.<br>
**Spirit-Infused** - Resistant to spirit damage and vulnerable to lightning damage. Heals itself on hits.<br>
**Poison-Infused** - Immune to poison damage. Explodes in a poison cloud on death.<br>
**Chaos-Infused** - One of the other infusions, randomly selected on each hit.

## Bosses
You can set a minimum and maximum level for bosses as well, if you want your bosses to spawn with up to five stars.<br>
There is also the option to let your bosses spawn with different affixes, making them even more difficult to kill:

**Reflective** - Dealing direct damage to the boss will deal damage to you as well<br>
**Shielded** - Takes 50% reduced damage from arrows<br>
**Mending** - Regenerates health over time more quickly<br>
**Summoner** - Summons strong creatures every 33% of maximum health lost<br>
**Elementalist** - Deals 20% increased elemental damage<br>
**Enraged** - Deals 20% increased physical damage<br>
**Twin** - Spawns a second boss. The boss and its twin boss have 25% less health and damage and have shared health.

## Loot
For loot, you can set a chance for additional loot with each creature level and set a multiplier for all dropped items as well. You can even let enemies drop multiple trophies, if you like. You can also let bosses drop more loot or multiple trophies.

## Multiplayer
For multiplayer, everyone in your group should have this mod, preferably with the same settings. Otherwise, the client controlling the spawn will be responsible for the level of the enemies. Also, you need this mod to see the actual level of the creatures or all enemies above 2 stars will just show up without any stars.

Or don't tell your friends about this mod, spawn some 5 stars Lox and tell them to parry them, while you are shooting from a safe distance using your bow. Watch them die and then laugh uncontrollably like the psychopath you are.

The mod has an option to adjust the HP and DMG increase for creatures per player in multiplayer.

And be mindful with the settings. If you spawn an entire Fuling village with 5 stars Fulings, changing the settings or disabling the mod will not revert their level.

## Synchronizing a configuration on a multiplayer server
You can install the mod on the server just like you would install it on the client as well (requires BepInEx on the server as well). If you do that, the server will automatically synchronize all settings, including the YAML configuration between all clients. There are two different modes that you can use:

**Locked Config** - Once you've started up the server with the mod installed, you will find a setting at the top of the configuration file, which looks like this:

	[0 - Server]

	## The configuration is locked and may not be changed by clients
	# Setting type: Toggle
	# Default value: Off
	# Acceptable values: Off, On
	Lock Configuration = Off


If you set this setting to 'On', the configuration will be locked and cannot be changed by clients. Opening the BepInEx Configuration Manager will display the servers configuration, but clients will be unable to change the configuration.

**Unlocked Config** - If you leave the setting mentioned above set to 'Off', clients can open the BepInEx Configuration Manager to change the configuration. Changing the settings there will synchronize the changes to all clients connected to the server immediately and update the configuration file on the server as well.

Both modes will not change the configuration file on your computer and your own configuration will be used, if you connect to a server that doesn't synchronize the configuration.


# I accidentally spawned a level 5000 creature / boss! What now?
If you have attached '-console' as a launch parameter for Valheim, you can open the console by hitting F5 in the game. The following command can be used, to remove accidentally spawned creatures:

	cllc killall
	
Removes all nearby creatures.


## Fun Features:
- Run away from giant Fuling Berserkers.
- Get killed instantly by Deathsquitos with 5 stars.
- Encounter 5 stars Serpents and curse the game, because the wind is against you and doesn't let you flee.
- Tame giant 5 stars Wolves and watch them devour your enemies!
- And so much more!
- (If you are only reading this list for some reason: Yes, you can use this mod to make the game A LOT easier.)


Need more stamina to fight tough enemies? Check out [this sweet mod](https://valheim.thunderstore.io/package/Smoothbrain/StaminaRegenerationFromFood)﻿ and make sure you are always [properly rested](https://valheim.thunderstore.io/package/Smoothbrain/ComfortTweaks)!