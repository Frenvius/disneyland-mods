# v1.0.3 - Update for 0.217.24
* Updates for 0.217.24 Valheim

# v1.0.2 - Small Update
* Fixing error messages that show up during spawn and death events.
  * The errors didn't effect operations.

# v1.0.1 - Small Update
* Fixing an inventory bug found in a rare scenario.
* New Container Protection Logic to ensure Tames don't destroy containers, if enabled.

# v1.0.0 - Initial Version of AutoFeedRedux
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
