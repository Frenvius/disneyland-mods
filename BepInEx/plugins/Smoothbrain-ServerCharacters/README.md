# Server Characters

Saves your character on the server, instead of your computer, to prevent you from messing with it.

Has to be installed on all clients and the server, to have any effect.

If you want to copy profiles from the client to the server manually, just copy them to the character folder on the server and prefix them with the Steam ID (for Steam save files) and an underscore.

## Features

### Crossplay

ServerCharacters works with the Xbox Gamepass version of the game as well.

### Backups

Creates backups of all profiles on the server automatically. Backups are saved in the same folder as the character profiles. Number of backups to keep can be configured.

### Emergency Backups

If a client suddenly loses connection to the server, it will automatically create an emergency backup, which it will upload to the server on the next connection, to restore it. This means that no progress will be lost, even if your internet breaks down or the server crashes for some reason.

These backups have a signature and messing with them will void this signature. The server will reject restoring emergency backups with an invalid signature.

### AFK Kick Timer

You can configure a time after which players will be automatically disconnected from the server, if they are AFK (= didn't move) for this time.

### Poison Debuff Storage

By default, poison debuffs on players are stored in the save file on logout and applied to the player on login. This prevents players from clearing their poison debuffs by relogging. This can be disabled in the config.

### Server Side Inventory

The inventory of all characters is saved on the server, to prevent players from duping items.

### Single Character Mode

You can toggle the single character mode on in the servers configuration file. If it's on, each SteamID can only create one character on the server. Does not apply to server admins.

### Console Commands

Server admins can use several console commands. The following commands are available right now.

ServerCharacters console commands - use 'ServerCharacters' followed by one of the following options.
- resetskill [skillname] [playername] [id] - resets the skill for the specified player. Steam / Xbox ID is optional and only required, if multiple players have the same name. If no name is provided, the skill is reset for every character on the server, online and offline.
- raiseskill [skillname] [level] [playername] [id] - raises the skill for the specified player by the specified level. Steam / Xbox ID is optional and only required, if multiple players have the same name. If no name is provided, the skill is raised for every character on the server, online and offline.
- teleport [playername] [id] - teleports you to the specified player. Quote names with a space. Steam / Xbox ID is optional and only required, if multiple players have the same name.
- summon [playername] [id] - teleports the specified player to you. Quote names with a space. Steam / Xbox ID is optional and only required, if multiple players have the same name.
- giveitem [itemname] [quantity] [playername] [id] - adds the specified item to the specified players inventory in the specified quantity. Quote names with a space. Steam / Xbox ID is optional and only required, if multiple players have the same name. Will fail, if their inventory is full.

### Backup Only Mode

You can toggle the backup only mode on in the servers configuration file. If it's on, the server will not enforce the server's character profile anymore.

### Hardcore Mode

You can toggle the hardcore mode on in the servers configuration file. If it's on, players will get kicked and their save file will be deleted from the server, if they die. They will still be able to keep the characters for singleplayer in this case.

### Character Templates

On the server side, you can create a file named CharacterTemplate.yml in the same folder that has the DLL for this mod. You can add a custom spawn point, items and skills to this file. New characters will have these items and skills and will spawn at the configured position.

Example:
```yml
items:
  Wood: 50
  Stone: 30
  
skills:
  Bows: 15
  Run: 20

# You can define as many spawn points as you want. If you have multiple spawn points, one will be picked randomly.
spawn:
  - x: 100
    y: 50
    z: 150
  - x: 200
    y: 150
    z: 350
```

### Maintenance Mode

Server admins can enable the maintenance mode. Once enabled, a timer starts. When this timer elapses, all characters will be saved, the world will be saved and all non-admins will be disconnected and cannot login until the maintenance mode has been disabled.

You can also enable the maintenance mode from the command line of the server, by creating a file named 'maintenance' in the same folder that the DLL is in. To disable it, simply delete this file. This can be used to enable the maintenance mode from the same script that does the server restart, to prevent players from losing progress.

### Discord Webhooks

In the configuration file on the server, you can set up notifications about maintenances and new players for your Discord server. These values are not synced and won't be visible on the clients.

### Linux Administration Webinterface

ServerCharacters has an API that can be used to connect a webinterface, to allow everyone to easily manage your Valheim server, even with no knowledge about Linux servers. Can also be used to do automated schedulded restarts of the Valheim server.

For a fully functional example webinterface, please see [my GitHub repo](https://github.com/blaxxun-boop/Webinterface).