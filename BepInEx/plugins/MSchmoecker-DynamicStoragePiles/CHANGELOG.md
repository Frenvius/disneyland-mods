# Changelog

0.5.1
- Fixed typo when an item cannot be placed in a container

0.5.0
- Added [StackedBars](https://valheim.thunderstore.io/package/Azumatt/StackedBars/) integration when both mods are installed
- Added the option to restrict containers to only accept items of the respective type, so wood piles only accept wood etc., enabled by default (thanks Searica)
- Changed mod enforcement, now both the server and all clients need to have the mod installed. This is to prevent desync issues with the new container restrictions
- Reworked config options, please update your settings as some old options are no longer used. To clean up unused options, remove the old config file

0.4.0
- Added [IngotStacks](https://valheim.thunderstore.io/package/MySoloTeam/IngotStacks/) integration when both mods are installed
- Added mod enforcement to all players if the mod is installed on the server
- Fixed compatibility with the AzuAutoStore 2.0.0 update

0.3.0
- Added the config option to disable vanilla stack pile recipes, making them not buildable with the hammer. Disabled by default
- Added explicit compatibility with AzuAutoStore, items are only stored into the respective stacks piles. Enabled by default
- Fixed ordering of the yggdrasil wood stack in the build menu

0.2.0
- Added coin pile
- Added custom icons for stacks and piles

0.1.0
- Release
