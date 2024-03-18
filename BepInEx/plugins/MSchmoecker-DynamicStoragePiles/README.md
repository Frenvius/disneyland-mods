# Dynamic Storage Piles

## About

Adds stacks and piles as new container pieces. Their appearance changes depending on the fill level.


## Features

Stacks and piles can be built on the hammer using 10 items of their respective material.
No workbench or other crafting station is required, they can be built anywhere.
Each stack has 10 slots that can be used to store any item.

Vanilla stacks and piles models are used:
- Wood stack
- Fine wood stack
- Core wood stack
- Yggdrasil wood stack
- Stone pile
- Coal pile
- Black marble pile
- Coin pile

![StackOverview](https://raw.githubusercontent.com/MSchmoecker/Dynamic-Storage-Piles/master/Docs/StackOverview.png)

Depending on the inventory fill level, more items will be displayed on the stack:

![StackOverview](https://raw.githubusercontent.com/MSchmoecker/Dynamic-Storage-Piles/master/Docs/StateShowcase.png)

### Mod Integration

This mod integrates both [IngotStacks](https://valheim.thunderstore.io/package/MySoloTeam/IngotStacks/) and [StackedBars](https://valheim.thunderstore.io/package/Azumatt/StackedBars/) as container stacks for ingots.
IngotStacks/StackedBars and DynamicStoragePiles must be installed for this to work, otherwise no ingot stacks will be added to the game.

Each stack costs 3 ingots of the respective material to build:
- Copper Stack
- Tin Stack
- Bronze Stack
- Iron Stack
- Silver Stack
- Black Metal Stack
- Flametal Stack

Example of dynamic IngotStacks:

![IngotStacksShowcase](https://raw.githubusercontent.com/MSchmoecker/Dynamic-Storage-Piles/master/Docs/IngotStacksIntegrationShowcase.png)

Big thanks to Richard and Azumatt for the awesome mods and possible integration!


## Manual Installation

This mod requires [BepInEx](https://valheim.thunderstore.io/package/denikson/BepInExPack_Valheim/) and [Jötunn](https://valheim.thunderstore.io/package/ValheimModding/Jotunn/).\
Extract the content of `DynamicStoragePiles` into the `BepInEx/plugins` folder or any subfolder.

The mod must be installed on the server and all clients for it to work.

## Other mods

### Related mods

- [IngotStacks](https://valheim.thunderstore.io/package/MySoloTeam/IngotStacks/), integrates with this mod if both are installed
- [StackedBars](https://valheim.thunderstore.io/package/Azumatt/StackedBars/), integrates with this mod if both are installed
- [Balrond Containers](https://valheim.thunderstore.io/package/Balrond/balrond_containers/)
- [ArborStorage](https://valheim.thunderstore.io/package/coemt/ArborStorage/)
- [Digitalroots GoldBars](https://valheim.thunderstore.io/package/Digitalroot/Digitalroots_GoldBars/)
- [OdinsFoodBarrels](https://valheim.thunderstore.io/package/OdinPlus/OdinsFoodBarrels/)


### Compatible mods

Most mods that change something about the vanilla containers should be.
The following mods are a few examples:
- [Automatic Fuel](https://valheim.thunderstore.io/package/TastyChickenLegs/AutomaticFuel/)
- [AzuAutoStore](https://valheim.thunderstore.io/package/Azumatt/AzuAutoStore/), explicit compatibility to only store items into the respective stacks, configurable
- [Quick Stack Store Sort Trash Restock](https://valheim.thunderstore.io/package/Goldenrevolver/Quick_Stack_Store_Sort_Trash_Restock/)


## Links

- [Thunderstore](https://valheim.thunderstore.io/package/MSchmoecker/DynamicStoragePiles/)
- [Nexus](https://www.nexusmods.com/valheim/mods/2527)
- [Github](https://github.com/MSchmoecker/Dynamic-Storage-Piles)
- Discord: Margmas. Feel free to DM or ping me about feedback or questions, for example in the [Jötunn discord](https://discord.gg/DdUt6g7gyA)


## Development

See [contributing](https://github.com/MSchmoecker/Dynamic-Storage-Piles/blob/master/CONTRIBUTING.md).


## Changelog
See [changelog](https://github.com/MSchmoecker/Dynamic-Storage-Piles/blob/master/CHANGELOG.md).
