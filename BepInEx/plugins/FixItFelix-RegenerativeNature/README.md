# Regenerative Nature

This mod contains some configuration that can be used to regenerate the nature from 
chopped trees and mined ores (at least a spawner for tin).

Other ore's spawners you can create yourselves easily using the given spawner and 
modifying it slightly. The names of some prefabs I found in the past for other ores
are contained in the file as comment already.

If you already use your own spawners for SpawnThat, make sure that the used 
IDs (197xx-199xx) don't colide with yours.

## Installation

For client-side only, just download this mod using TMM/r2modman from Thunderstore. 
This will do all necessary steps to use it out-of-box.

To use this, you will need to also use SpawnThat (linked as dependency).

For manual installation you will need to download the dependencies yourself and put
plugins contents from them into you BepInEx plugins folder and the contents of 
"config" folder of this mod into BepInEx's config folder.

If you want to use this on a server that uses SpawnThat already, the server 
needs to have the config files loaded, too, since it will sync with clients.

## Changelog:

* 1.2.3: smaller version updates, no content changes
* 1.2.2: moved the spawner IDs all to sub of 19xxx to have less conflict chances with other mods configuring spawners
* 1.2.1: fixed altitude for seeds
* 1.2.0: also added the rare seeds like turnip to be spawned more often; slight improvement for tin
* 1.1.0: version updates only
* 1.0.3: with the fixes coming with SpawnThat 0.11.x the spawning of trees and ores is also fixed and proved working well - no mass spawning without respecting distances will happen anymore. Also adjusted altitude settings, since some were out of range.
* 1.0.0-2: forgot the changes... :)

## Contact

* https://github.com/FelixReuthlinger/regenerative-nature
* Discord: Flux#0062 (you can find me around some of the Valheim modding discords, too)
