### 1.15.1
- Corrected behaviour of [Crops]EnemiesTargetCrops. When disabled, mobs will definitely no longer attack your crops.

### 1.15.0
- Moved localization & ExtraResources.cfg files to the config folder.
- Added [Difficulty]EnemiesTargetPieces & [Crops]EnemiesTargetCrops.
	- When false, mobs won't attack pieces or crops placed with the cultivator.
- Removed hammer's ability to remove cultivator pieces.
- Fixed dupe exploit when RecoverResources is enabled.

### 1.14.1
- Fixed NRE when a custom ExtraResource has a Pickable component and [General]ShowPickableSpawners is enabled.

### 1.14.0
- Updated for Valheim v0.217.22.
- Compiled against BepInEx 5.4.22.
- Updated ServerSync to v1.15.
- New feature and config option: [General]EnableExtraResources.
	- When enabled, users/server admins can define any prefabs (even from other mods) to add to the cultivator build table. This feature will be expanded upon in future updates.
- New config option [General]DisabledResourceNames.
	- Specific resources added by the mod can now be modularly disabled.
- Added autumn birch sapling (plains variant).
- Misc code improvements.

### 1.13.7
- Updated for Valheim v0.217.14 (Hildir's Request).

### 1.13.6
- Updated for Valheim v0.216.9.
- Rebuilt embedded asset bundle for Unity 2020.3.45f1.
- Removing pieces with the cultivator will now play piece specific SFX.
- Removing pickable objects with the cultivator will now drop its resources before being destroyed.

### 1.13.5
- To avoid confusion and to make things more intuitive, [Crops] and [Seeds] categories will no longer display in the BepInEx Configuration Manager unless their respective overrides, EnableCropOverrides and EnableSeedOverrides, are set to true.

### 1.13.4
- Compiled against Valheim v0.214.305.
- Fixed default min and max growth scale for vanilla saplings.

### 1.13.3
- Updated for Valheim v0.214.2.
- Compiled against BepInEx 5.4.21.0.
- Fixed growth remaining hovertext formatting bug that was introduced with latest Valheim update.

### 1.13.2
- Ancient and Ygga Saplings can now grow in any biome when EnforceBiomes is disabled.

### 1.13.1
- Removed meadows restriction on decorative pieces when EnforceBiomes is enabled.
- Omitted black cores from respawn time display.
- Fix for Unity Exception when running in development mode.
- Miscellaneous code optimizations and reduction of mod footprint.

### 1.13.0
- Trees & Seeds update!
- Added ygga saplings.
- Gave ancient saplings a unique appearance.
- Added [Seeds] config options TreeDropMin & TreeDropMax.
- Corrected [Seeds] setting descriptions.
- Fixed benign NRE when leaving game while viewing plant growth progress.

### 1.12.0
- Updated for Mistlands v0.212.7.
- [Crops] configuration options added for, and now apply to, jotun puffs and magecap.
- Added small ygga tree recipe to the cultivator.
- Added 2 new [Crops] settings, CropsRequireSunlight & CropsRequireGrowthSpace.
	- Greenhouses?

### 1.11.7
- Updated ServerSync to v1.13 for Valheim 0.211.11.

### 1.11.6
- Updated ServerSync to v1.11 for Valheim 0.211.7 crossplay support.

### 1.11.5
- Fixed null reference error that occurs when an ancient sapling matures into a tree while PlaceAnywhere is enabled.

### 1.11.4
- Fixed localized text for BlueberryBush build description.

### 1.11.3
- Fixed [Crops]OnionReturn using value set in OnionCost.
- Ensured plant growth times are set to a minimum 10 seconds.
- [Difficulty]ResourcesSpawnEmpty now applies to all pickables.
	- Applies to berry bushes, mushrooms, flowers, and debris.
- Updated to ServerSync v1.6.

### 1.11.2
- Fixed collision on dandelions.

### 1.11.1
- Added new icons for all added pieces in the cultivator menu to match vanilla art style.
- Removed [General]AlternateIcons config option.
- Added 3 new buildable pieces: Branch, Stone, and Flint debris.
- New config category 'Debris', including 6 new settings.

### 1.11.0
- At long last, with 3D modeling assistance from Bento, custom meshes for picked flowers and mushrooms are finally here.
	- Added custom meshes for picked flowers and mushrooms.
- [General]AlwaysShowSpawners has been removed in place of ShowPickableSpawners (defaults to true) which can be toggled off to restore vanilla behaviour.
- Added toggleable snap points for vines.
- Updated some config descriptions.
- Misc improvements.

### 1.10.1
- Toggling [Crops]EnableCropOverrides off while in game now correctly un-applies all [Crops] settings.

### 1.10.0
- Removed custom AncientSeeds item.
	- Planting an Ancient Sapling now requires a vanilla AncientSeed.
- Added Cost and Return config settings for individual crops.
- Added extra null reference prevention.
- Compiled against BepInEx 5.4.19.0.
- Moved [Difficulty]EnableCropOverrides to [Crops].
- Added EnableSeedOverrides to [Seeds]
	- Must be enabled for [Seeds] config options to be applied.

### 1.9.2
- Fixed incompatibility with Better Creative, with fix submitted by its author, Heinermann.

### 1.9.1
- New config category: UI.
	- Moved EnablePickableTimers to UI category.
	- Added [UI]EnablePlantTimers and [UI]GrowthAsPercentage.
- Growth time remaining can be seen as hover text on crops, saplings, and pickables, and optionally may be displayed as a percentage.

### 1.9.0
- Adopted ServerSync in place of Authoritative Config.
- Changes to configuration options while in game, through BepInEx Configuration Manager or synchronization with connected clients, will immediately take effect without a world reload.

### 1.8.6
- Berry bushes, mushrooms, and flowers can now individually have their recipes removed from the cultivator by setting their respective resource cost to 0 in the configuration file.

### 1.8.5
- Added extra null reference error prevention.
- Compiled against BepInEx 5.4.1601 and Valheim 0.205.5.

### 1.8.4
- Fixed bug where some trees would only drop one or two items from their drop table, even when [Seeds] oneOfEach was set to true.

### 1.8.3
- Added [Seeds] configuration options category with 4 new settings.
	- These settings normalize the amount of seeds that drop from the various tree types, and allow the user to define seed drop rates and amounts.

### 1.8.2
- Fixed ancient trees having no placement cost.

### 1.8.1
- Updated for Valheim v 0.202.14 (Hearth & Home).
- Removed config options [Saplings] BirchCost, OakCost, AncientCost.
- Removed custom Birch/Oak seeds and saplings (included now in base game).

### 1.8.0
- Added [General] EnablePickableTimers config option (defaults to true).
	- When enabled, pickables will display growth time remaining in hover text.
- Added large glowing mushroom recipe to cultivator.

### 1.7.1
- Cultivator can now remove branch, stone, and flint spawners using the deconstruct key.

### 1.7.0
- Redesigned the PlaceAnywhere config setting.
- When PlaceAnywhere is enabled, the following changes take effect:
    - Saplings, small trees, and bushes can be placed indoors.
    - Saplings can grow into trees indoors, and sapling grow radius is ignored.
    - Bushes and saplings/trees placed while PlaceAnywhere is enabled will defy gravity.
        - (to prevent them from falling through floors).
    - Even if PlaceAnywhere is later disabled, the pieces will continue to float until the world is loaded without the mod present.

### 1.6.3
- Rebuilt embedded asset bundle for Valheim 0.155.7.
- Fixed monster AI targeting non-player built flora after 0.155.7 AI changes.

### 1.6.2
- Added config option [Difficulty] : ResourcesSpawnEmpty (defaults to false).
    - When set to true, berry bushes will spawn without fruit when placed.

### 1.6.1
- EnforceBiomes config option now correctly applies to saplings.
- Fixed cultivator not animating when deconstructing vines.

### 1.6.0
- Cultivator can no longer remove all building pieces, only pickables and vines.
- Deconstruct now respects ward permissions.
- Added vfx and sfx when removing vines.
- Added config option, RecoverResources, to the [Difficulty] section of config (off by default).

### 1.5.2
- Updated for Valheim 0.154.1.
- Removed respawn time fix for pickable resources (fixed in base game).

### 1.5.1
- Added CropsRequireCultivation config option to [Crops] section (defaults to true).
- Fixed logic for PlaceAnywhere and RequireCultivation config options.

### 1.5.0
- Added new server authoritative config options to override grow radius, growth time, and scale of crops.
- Improved compatibility with other mods that cause game code to execute earlier than expected.

### 1.4.3
- Added chance for birch sapling to spawn autumn (plains) leaf variants.
- Added AlwaysShowSpawners config setting.
    - When enabled, spawners for mushrooms, thistle, and dandelion will remain visible after being picked.

### 1.4.2
- Birch trees found in the plains can now drop birch cones.
- Added config options for modifying growth time and min/max scale of beech, pine, and fir saplings.
- Centralized debug log source for tidier logging.

### 1.4.1
- Correctly adds cultivator recipes after receiving authoritative config.

### 1.4.0
- Added several new buildable pieces to the cultivator that can be enabled/disabled with new config option EnableMiscFlora (on by default).
- New config options to control grow radius of all tree saplings.
- Misc performance and code improvements.
	
### 1.3.3
- Fixed mod not initializing when connecting to a server that isn't hosting the mod.
- Fixed BirchCost, OakCost, and AncientCost config options not taking effect.
	
### 1.3.2
- Reverted to 1.2 method of adding cultivator recipes.
    - Hopefully this addresses the problem some people were experiencing with 1.3.
	
### 1.3.1
- Server configuration settings are now properly authoritative when enabled.
- Configuration options are now re-applied each time a world is loaded.
	
### 1.3.0
- Dropped MCE support.
    - Mod now uses Authoritative Config for server config synchronization.
	
### 1.2.2
- Fixed small beech and fir trees disappearing. Improved MCE support.
	
### 1.2.1
- Re-fixed functionality of EnforceBiomesVanilla config option.

### 1.2.0
- Added ability to plant small fir and beech trees.
- EnforceBiomesVanilla config option now allows barley and flax to grow outside of the plains.
- Added localization support (see mod description for details).

### 1.1.0
- New icons for berry bush pieces and placeholder icons for seed items.
- Corrected DandelionRespawnTime config description.
- Added EnforceBiomesVanilla option (default true).
- Optimizations: reduced mod footprint.

### 1.0.0
- Created Mod.