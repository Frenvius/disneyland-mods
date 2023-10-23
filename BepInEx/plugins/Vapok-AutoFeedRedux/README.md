# AutoFeedRedux by Vapok

AutoFeederRedux is a completely re-engineered take on the auto feeder. Reduces the amount of looping that other feeders were doing, and does not need to keep track of every container.

Out of the box settings, containers near tameable creatures, will be used for feeding if there is an appropriate food for that tame in the box.

The following settings are customizable:
* Feed Range - Default: 10 meters
  * Range in Meters that creatures will attempt to eat from container.
* Require Move - Default: Enabled
  * Requires creatures to move closer and within the proximity of the container in order to feed.
  * Setting to Disabled will feed the creature automatically without having to move it assuming it is within the Feed Range.
  * This setting is not fool-proof, and large distances are difficult to navigate. Advice is to ensure you are putting your tames in a pen.
* Move Proximity - Default: 5f
  * The maximum distance from the container it will allow to feed if required to move.
* Disallow Feed - Default: <empty>
  * This is a comma-separated list of food that you want to prevent tames from eating from a container automatically.
    * Acceptable values: Carrot,Turnip, etc.
* Disallow Animal - Default <emtpy>
  * This is a comma-separated list of creatures that you do not want to auto-feed.
    * Acceptable values: Boar,Lox, etc.
* Protect Containers - Default: true
  * When enabled, creatures in the taming process will be highly encouraged to not attack nearby containers with food in them.
  * This greatly reduces the frequency that creatures, while taming, will attack the containers.

### Mod Author Details

Author: [Vapok](https://github.com/Vapok)

Source: [Github](https://github.com/Vapok/AutoFeedRedux)

Discord: [Vapok's Mod's Community](https://discord.gg/5YAJkRFBXt)

Patch notes: [Github Patchnotes](https://github.com/Vapok/AutoFeedRedux/blob/main/PATCHNOTES.md)


