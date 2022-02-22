## This Mod adds 3x wearable backpacks to the game

#### This mod comes with 3x wearable bags, The concept was to replace Jotunn backpacks as the code for that mod is no longer being maintained;

### The bag types this includes is:
 1) Leather Bag. This bag has a small number of slots and can be crafted early on in the game with some DeerHide and LeatherScraps.
 2) Iron Bag: This bag has quite a few more slots to keep your things in. It requires Iron to craft so you have had to make it to the swamps to see this one !
 3) Silver Bag: This bag is probably the nicest one you can make. It has the largest capacity


Some details about the bags.
All bags have dynamic inventory that is per bag per world.
You can't store a bag in a bag.

You can't teleport with unteleportable items in your bag even if you unequip your bag and stick it in your inventory. 

This mod also has support for Jude's equipment. If you have that mod installed the backpacks from Jude's equipment will now have inventories you can interact with.

This mod is a ServerSync'd mod and is required to live on the server as well as the client who uses it.

To bring up the bag's inventory you must 
1) Have bag equipped
2) Have inventory up and visible
3) Press LeftShift + E 
4) View bag contents


#### Huge thanks to:
* Blaxxun - Code Contribution
* Evie (CinnaBun) - BackPack Models
* DeBarba - BackPack Model


# KNOWN CONFLICTS!
1) Jotunn BackPacks
2) Reported Conflict with OdinQOL when using increase inventory size

If you get any conflicts/Issues please find me in the Odin+ Discord


### V0.0.8
* Added Config options for carry capacity bonus [Server Synced]
* Added config options for movement speed modifier [Server Synced]
* Added config for carry weight buff [Server Synced]
* Added UI Tooltip for how to open bag inventory when it is equipped
* Added code to increase bag slot count based on bag level the more levels the more slots
* Fixed recipes for bags not matching tiers


### V0.0.9
* Fixed Leather move speed config not working

### V0.1.0
* Fixed dissappearing bag inventory
* Fixed reported logspam in 0.0.9 via github issue
* Fixed SE_Stat showing odd name in corner of screen (should show nothing)

### V0.1.1
* Added weight modifier to the description of the bag
* Fixed SE icon showing when bag equipped 

### V0.1.2
* Fixed edge case item dupe bug
* Fixed game crash when unequip bag while viewing its inventory
* Fixed inventory loss on bag upgrade (bags now retain stuff when you level them up)
* Added modifier info the description of bag <img src="https://user-images.githubusercontent.com/67915879/154521277-a89f2893-fadd-42ec-858b-ceacf7ef0417.png">

### V0.1.3
* Fixed incompatibility with EAQS by RandyKnapp
* Fixed initial bag load issue when equipping bag of same type but different level yielding incorrect size
* Altered Teleportation check logic, Now when any bag holds something that is not teleportable. The bag itself becomes unteleportable.
* Altered CarryWeight modifier logic to actually apply 
* Fixed dynamic bag slot growth based on bag quality level applying

### V0.1.4
* Fixed reported conflict with Dual Wield

### V0.1.5
* Fixed issue where Jude's bags had no inventory displayed


### V0.1.6
* Fixed issue with teleportation while holding a bag

### V0.1.7
* Fixed issue when upgrading bag and having equipped inventory slot size did not increase
* added configuration values for bag starting sizes
* added configuration value for key to open bag 

### V0.1.8
* Fixed issue with Judes bags not grabbing slot size
* Fixed issue where if you didnt edit bag contents and unequipped it was not saved

### V0.1.9
* Fixed issue if you store bag in Chest and logout the bags weight was reset
* Fixed Auga compatibility
* Added Auga tooltip for how to equip bag
* Added Russian and German translations (Thank you SorXchi && Blaxxun)

### V0.2.0
* Fixed reported null reference (red text) when loading new world or moving too fast in your world 

### V0.2.1
* Fixed improper manipulation of scriptable object when deploying the carrybuff SE
