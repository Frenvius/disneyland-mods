A server and client side mod to force show position on the map. Can join servers that do not have this mod installed, with this mod installed.

`Install on all clients and the server.`

`This mod uses ServerSync, if installed on the server and the config is set to be forced, it will sync all configs to client`

`This mod uses a file watcher. If the configuration file is not changed with BepInEx Configuration manager, but changed in the file directly on the server, upon file save, it will sync the changes to all clients.`

> ## Configuration Options
`[1 - General]`

* Lock Configuration [Synced with Server]
  * If on, only server admins can change the configuration.
    * Default value: On
* Prevent Public Toggle [Synced with Server]
  * Prevents you and other people on the server to turn off their map sharing option. NOTE: If the admin exempt toggle is on, admins bypass this.
    * Default value: On
* Admin Exempt [Synced with Server]
  * If on, server admins can bypass the force of position sharing.
    * Default value: On
* Off In Wards [Synced with Server]
  * If on, hide position sharing in wards. NOTE: This will force position to toggle off and stay off while inside a ward.
    * Default value: Off


> ## Installation Instructions
***You must have BepInEx installed correctly! I can not stress this enough.***

#### Windows (Steam)
1. Locate your game folder manually or start Steam client and :
   1. Right click the Valheim game in your steam library 
   2. "Go to Manage" -> "Browse local files"
   3. Steam should open your game folder
2. Extract the contents of the archive. Put the DLL into BepInEx\plugins the other files are needed for the thunderstore upload and can be ignored.
3. Locate azumatt.WhereYouAt.cfg under BepInEx\config and configure the mod to your needs

#### Server

`Must be installed on both the client and the server for syncing to work properly.`
1. Locate your main folder manually and :
   1. Extract the contents of the archive into BepInEx\plugins.
   2. Launch your game at least once to generate the config file needed if you haven't already done so.
   3. Locate azumatt.WhereYouAt.cfg under BepInEx\config on your machine and configure the mod to your needs
2. Reboot your server. All clients will now sync to the server's config file even if theirs differs.


`Feel free to reach out to me on discord if you need manual download assistance.`



# Author Information

### Azumatt

`DISCORD:` Azumatt#2625

`STEAM:` https://steamcommunity.com/id/azumatt/


For Questions or Comments, find me in the Odin Plus Team Discord or in mine:

[![https://i.imgur.com/XXP6HCU.png](https://i.imgur.com/XXP6HCU.png)](https://discord.gg/Pb6bVMnFb2)
<a href="https://discord.gg/pdHgy6Bsng"><img src="https://i.imgur.com/Xlcbmm9.png" href="https://discord.gg/pdHgy6Bsng" width="175" height="175"></a>
***
> # Update Information (Latest listed first)
>
> ### v1.0.7
> - Mistlands Update
> ### v1.0.6
> - Update ServerySync internally
> ### v1.0.5
> - Update ServerySync internally
> - Update WIL compatibility naming for new GUID.
> ### v1.0.4
> - Update ServerSync internally
> - Make sure error on version mismatch is bigger
> ### v1.0.3
> - WIL compatibility update for WIL v3.0.1
> ### v1.0.2
> - Version string issue fix.
> ### v1.0.1
> - Attempt at fixing version string load.
> ### v1.0.0
> - Initial Release