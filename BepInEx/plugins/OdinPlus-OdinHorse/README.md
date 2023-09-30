<p align="center"><img src="https://i.imgur.com/wlKugPa.png" alt="Horse"></p>
<p align="center"><img src="https://i.imgur.com/QlFqCK7.png" alt="Horse"></p>
<p align="center"><img src="https://i.imgur.com/XNHUnIX.png" alt="Horse"></p>
<p align="center"><img src="https://i.imgur.com/GK3foLS.png" alt="Horse"></p>

# OdinPlus Mod Team Presents: Horse
**Produced by: Raelaziel#0954**

## About Horse

Horse is just simple custom creture mod with new items. You can tame it, You can ride it, he even got continers like horse bag to stash items

In case of anything: You're using this mod on your responsibility, make sure you did backup of your character/world.

## News & Important info.

⚠️**Warning! Please delete old `.cfg` file and generate new one!**

If you are interested in cooperation, create your own objects that you would like to see in the game, have any ideas or questions, or even make Your own mods then join our OdinPlus Discord Channel, if you want to chat with our team, find us on:
https://discord.gg/mbkPcvu9ax

# You like my mods? ❤️Donate me.
Your donation will help me alot! Thank you!<br>
https://www.paypal.com/paypalme/raelaziel<br>

## Custom Creature - Horse

### Short info.

- Horse will spawn on Meadows, he's pretty rare to find as he spawns only on Sunny Days
- Horse will no more have bag, but now You can attach the Cart! Thanks to cLevel (jcleveland)
- Horse can be tamed with Blueberries, Carrots, Cloudberries and Barley 
- Horse offspring will run away from You so make sure to close it carefully
- Growth and taming time is quite same as Lox
- **Everything from above is configurable for this moment!**

### Creatures and items
Every item start with `"rae_"` prefix so if you want to spawn them just use it to find all items

- rae_OdinHorse - horse prefab
- rae_Offspring_Normal - horse offspring prefab
- Horse Hide - basic material
- Horse Meat - basic food material
- Horse Trophy - horse trophy
- Horse Saddle - basic item required to ride the horse
- Horse Helmet - new helmet with Set condition
- Horse Cape - new cape with Set condition
- Horseaker Axe - new two-handed axe with Set condition
- Horse Rug piece - new rug to build with hammer
- Horsie piece - new chair, thanks GraveBear
- Horse Meat Skewer - new food
- Soup from Horse Meat - new food
- Horse Sticks - new food

## Installation (how-to)

Place the files to your `/BepInEx/plugins/` folder.
You can setup folder OdinHorse should be placed into `/BepInEx/plugins/`

### Dependencies

This mod isn't standalone, to make it work properly you will need some other mods or tools called dependencies so make sure that everything is installed as it should. To make it work properly you need 1 hard dependency.

* BepInEx Valheim

## Configuration 

Configuration file will be generated after first launch with `OdinHorse.dll` properly installed into `/plugins/` folder!

Mod support custom localization, to make it work just copy the file `OdinHorse.Polish.yml` change the language to yours and translate the content inside the file. You can use some basic editors like Notepad or Notepad++.

Mod have Server-Sync implemented and there's possibility to modify basic configuration values like:

for `Creature`: Simple and basic creature settings<br>
for `Spawn`: Every spawn condition and more<br>
for `Items` and `Food`: Every basic crafting conditions

## Greetings

* Azumatt for Piece Manager and big help
* Blaxxun for Creature Manager and Item Manager
* Zarboz and GraveBear for OdinPlus Team and channel and help with Horse development
* DorlickTheDerelict, Sebaugar, Pavlo and everyone who was testing!
* OdinPlus Channel

## Contact

via Discord channel of OdinPlus or - Raelaziel#0954

# Changelog

### 1.1.0
- Added pins for Horse and new Cart - once object is loaded (You're close enough too Horse or Cart) it will show up in the minimap
- Added new, bigger Cart which is attachable to Horse but too heavy to be used too drag with Player, have more slots and 2 sitting places
- Removed full armor shown when Horse is saddles
- Fixed SFX for Horse walking and running

Thanks much for KG for adding Pin function!

### 1.0.1
- Fixed problems with configs not being properly described
- Reduced mod size ~ Thanks GraveBear for tips
- Fixed visuals with Horse helmet which shouldn't be visible
- Fixed "walking" animations
- Fixed `CanBeTamed = 0` config, it's now configured properly
- Increased Running speed
- Increased Health
- Increased Stamina
- Above tweaks are just configs, you can change them in .cfg file

### 1.0.0
- Mod was secured with KeyManager. Need to be tested on Dedicated server
- Recompiled with latest game version
- Updated LocalizationManager
- Updated ItemManager
- New configuration options thanks to the latest ItemManager
- Updated PieceManager
- Reduced mod size
- Cleared project - thanks Blaxx
- Fixed some of localization

- Added new configuration setting - Running Speed

### 0.5.5
- Updated ServerSync
- Added Vulcan Support

### 0.5.1
- Precompiled Yaml which will fix latest error
- Added German translation file. Thanks `Markusgo1967`

### 0.5.0
- Implemented LocalizationManager
- Localization is now inside `OdinHorse.English.yaml` file. You can copy this file and translate the content for you own needs, just change the language name like `OdinHorse.YourLang.yaml`
- Turned off Offspring spawn as default as that wasn't good idea. Not only because of problems with errors but also about logic. Offsprings shouldn't spawn freely.

#### Here it comes!
- Added new configuration for Horse Health                  
- Added new configuration for Horse Stamina                 
- Added new configuration for Horse Stamina Regen            
- Added new configuration for Horse Stamina Regen when Hungry      
- Added new configuration for Horse Feeding Time             
- Added new configuration for Horse Taming Time              
- Added new configuration for Horse Offspring Health         
- Added new configuration for Horse Offspring Growup Time     
- Added new configuration for Horse Offspring Meat Drop Chance 
- Added new configuration for Horse Offspring Meat Drop Minimum
- Added new configuration for Horse Offspring Meat Drop Maximum
- Added new configuration for Horse Offspring Hide Drop Chance 
- Added new configuration for Horse Offspring Hide Drop Minimum
- Added new configuration for Horse Offspring Hide Drop Maximum

### 0.4.0
- Compiled with latest Valheim Patch 0.209.10
- Compiled against latest BepInEx
- Updated CreatureManager
- Updated ItemManager
- Offspring spawn configuration is back (delete and regenerate the config files)
- Decreased default hide and trophy drop from horse (configurable)
- Decreased default spawn rate of both, Horse and Offspring (configurable)
- Updated mod page

### 0.3.3
- Removed backpack to avoid Gravestone and items disapearing and NRE's
- Halfed the interval for Horse to give any sounds
- Added the mass for proper Cart usage
- Increased stamina regen when hungry
- Horse is commandable again

### 0.3.2
- Fixed Horse Offspring lack of parent - causing NRE's

### 0.3.1
- Fixed mod description

### 0.3.0 Extra Content
Added new items, foods, weapon and piece
Every item start with "rae_" prefix so if you want to spawn them just use it to find all items

- Horse Hide - basic material
- Horse Meat - basic food material
- Horse Trophy - horse trophy new model (slice from original model)
- Horse Saddle - basic item but with new model (from horse)
- Horse Helmet - new helmet with Set condition
- Horse Cape - new cape with Set condition
- Horseaker Axe - new two handed axe with Set condition
- Horse Rug piece - new rug to build with hammer
- Horsie piece - new chair KEKW, thanks GraveBear
- Horse Meat Skewer - new food
- Soup from Horse Meat - new food
- Horse Sticks - new food

### 0.3.0 Basic Content
Old project was lost and this horse was done from scratch. Take a note that this one can be different. Existing Horse should not disappear but check this out by your own before updating it on your multiplayer server.
Horse will be released in more variants just when all bugs and problems will be found and fixed

- Implemented new Creature, Item and Piece Managers by Blaxxun & Azumatt
- More configurables for Horse, Items and Pieces
- Horse texture is back from 0.1.0 release, so it's "Black Tobiano Pinto"
- New turning animations making horse behaves more naturally
- Reconfigured animations of walking and gallop
- Reconfigured acceleration. Horse is now accelerating slower
- Decreased turning angle limit so horse can't yeet 180 right now out of nowhere
- Disabled bag visual
- Increased stamina, stamina regeneration
- Decreased stamina burn for walking and gallop
- Reduced time needed for taming and time for breeding the Horse
- Added ragdoll (still need tweaks but it's something, ain't much but honest work)

### 0.2.0
Note that if one horse will not work properly i will not make more variations, fundament need to be solid to doo that
Horse will be released in more variants just when all bugs and problems will be found and fixed

- Implemented new CreatureManager by Blaxxun
- New complete config which will allow You to configure every spawn setting and more
- Changed Horse main texture for Meadows
- Changed spawn rate and interval
- Bag shouldn't randomly pops in, it's just disabled but container exist
- Added footsteps for walk, gallop, rear-up and kicks animations
- Removed attack completely, Horse will just stand-up on rear legs but will not do any damage
- Reduced interval for random idle sound
- Reduced time needed for taming and time for breeding the Horse
- Horse will now eat: Blueberries, Carrot, Cloudberry, Barley
- Reduced Health to 120 health points
- Reduced stamina (not final redo. i think, need more feedback)
- Changed faction to ForestMonster (from Animal Veg) so Horse will no longer attack BlackForest and Meadows monsters
- Horse will not "attack immediately" (Rear-up animation), should be more realistic
- Added Horse Head Trophy as test version

### 0.1.0
- Alpha Release

<p align="center"><h2>Find Raelaziel in the Odin Plus Team on Discord:</h2></p>
<p align="center"><a href="https://discord.gg/mbkPcvu9ax"><img src="https://i.imgur.com/Ji3u63C.png"></a></p>