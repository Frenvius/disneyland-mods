# Purpose

A minor anti-dickhead mod. Server files dictate what is allowed. Admins/Moderators bypass the check for
plugins.

```
Must be installed on all clients and the server.

Version checks with itself. If installed on the server, it will kick clients who do not have it installed.

This mod uses ServerSync, if installed on the server, it will sync all configs to client

This mod uses a file watcher. 
If the configuration file is not changed with BepInEx Configuration manager, but changed in the file directly on the server, upon file
save, it will sync the changes to all clients.
```

# Video Explanation v4.0.0 (and later!) (Click Image!)

[![AzuAnticheat Demonstration Video (v4.0.0)](https://i.imgur.com/Vpw39Il.png)](https://youtu.be/8dGZ1OLkmNE)

## Disclaimer

I do not claim that this will block all cheats, especially for those that are more tech-savvy than the average user.
Therefore, if you do some hacky things to bypass this, you can either help fix it or not claim it's a bug/issue. This
mod attempts to block and help maintain quality of life on a server that prefers to check for as much cheating as they
can. The game is client authoritative, I cannot check for everything the client might do.

## Features

* Logging to your discord using the Azumatt.AzuAntiCheat_Webhook.yml file
* Checks for common cheats activated in-game
* Can check for WeMod, CheatEngines etc.
* Whitelist folder on the server to dictate which mods the client connecting is allowed to use.
* Individual configurations for Moderators found in the Azumatt.AzuAntiCheat_ModeratorList.yml file

## Admin Only

* Can cheat and bypass DLL/Plugin Checks freely. Though, if a mod does its own version checking with the client, they
  still might be required to have the mod installed.

## Moderator

* Only bypasses DLL/Plugins by default. Can't activate common cheats or use cheat engines unless allowed by the server
  configs.

***
For Questions or Comments, find me in the Odin Plus Team Discord or in mine:

[![https://i.imgur.com/XXP6HCU.png](https://i.imgur.com/XXP6HCU.png)](https://discord.gg/Pb6bVMnFb2)
<a href="https://discord.gg/pdHgy6Bsng"><img src="https://i.imgur.com/Xlcbmm9.png" href="https://discord.gg/pdHgy6Bsng" width="175" height="175"></a>