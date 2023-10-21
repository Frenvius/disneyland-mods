## v4.3.1
- Quick fix for the new Valheim version
## v4.3.0
- Remove KeyManager from the mod. It is no longer needed and I do not care to keep it.
- Tweak some internals
## v4.2.0
- Update for the current Valheim version
- Add Spanish localization
- Fix the duplication of localization files because of the whitelist/greylist. If yml files or json files are found in these folders, they will be deleted automatically.
    - Also, I made a pull request on GitHub (that was accepted) to LocalizationManager to help fix this issue for all mods that use it. No more localization files causing your server to crash!

## v4.1.0
- Update for the current Valheim version
- Add the version the client is running to the logs/discord hook when kicked for mismatched mods.

## v4.0.0

- Please note that the configuration files will now be prefixed with Azumatt to be in line with my other mods.
  Example `Azumatt.AzuAntiCheat_Webhook.yml`
  , this means your old files can be renamed or you need to refill out the new files. This will be the last change I
  make to the file names.
- Recoded a lot of things to make it more simple, in doing so, I might have created some bugs I haven't found. Please
  never forget to join my discord and report them! (or DM me!) [My Discord](https://discord.gg/FcXwed7pZd)
- The mod can be used 100% in singplayer now. Shouldn't be any errors or issues.
- Make client disconnects faster when they have a mismatch or missing mod.
- Whitelist and Greylist generation no longer require a client boot of the game. This also means the previous myMods.yml
  will not be generated on the client
    - There will be two new folders generated inside your BepInEx/config folder on the server `AzuAntiCheat_Greylist`
      and `AzuAntiCheat_Whitelist`
        - Inside of these folders you will put the dlls that you would like to greylist or whitelist (folder respective)
          .
          The lists now generate automatically for your server.
          Allowing for "remote" admins to update their lists by simply downloading a mod and uploading it to the list
          folder they wish.
        - FAQs:
            - **What about the old greylist and whitelist yml files?** _You can delete them if you wish. They are no
              longer
              used._
            - **Why the config folder?** _Any mod put into the plugins folder would load on the server, which isn't
              needed if
              the mod is a client only mod._
            - **Why not just have the server generate the lists?** _Because the server doesn't need all the client dlls,
              and
              the client doesn't always need the server dlls._
            - **Does this mean my server will now need the same dll in both the config folder and plugins folder?**
              _Yes,
              but, the server will only need the dll in the plugins folder if the mod needs to be loaded on the server._
            - **Why can't I delete a file from the whitelist folder?** _This could be because you have some controls set
              in place that you cannot delete the files while they are being read. This typically happens on Windows
              machines_
            - **I am getting an error when moving my modpack to the server.** _My recommendation is, if you have to move
              a big number of mods to the server, to do it in small batches. This will prevent the server from locking
              the files or causing issues with reading them. Optionally, you can have the server off to avoid the issue
              altogether_
- Formatting changes on the damage value output.
- Discord output formatting changes.
- Localization changes.
    - Client output is now further localized.
    - Discord output can now be localized depending on your server's language. Change that value in the config. Found in
      section "1 - General"
        - If you have a language you would like to add, please submit a file to me and I will add it to the next
          release.
        - Please note: The discord output can be different from what the client sees. Meaning, the server can output a
          discord hook in German, but the client will still see the English version if their local language is set to
          English.
    - If you want to add additional localizations, you just have to create a file with the name `ModName.Language.yml`
      or `ModName.Language.json` anywhere inside of the BepinEx folder.
      For example, to add a Korean translation to this mod, a user could create a `AzuAnticheat.Korean.yml`
      file inside of the config folder and add Korean translations there.

## v3.0.0

- Fixed issues where cheaters could cause hash collisions or keep the hash the same when only modifying dlls, while not
  recompiling them.

## v2.1.0

- Fixed the log errors in SP.
- Fix the newly created (from whatever mod, not sure still) logout issue where logging out is delayed for too long and
  the AC kicks you. Due to the admin variable being reset on logout.
- Fixed the empty GreyList issue. Previously if your GreyList was empty, it would have issues kicking the client.
- Fix no discord output and the log error on the server when a user has a mod mismatch
- Localization fixes on some of the error outputs. Forgot to localize them correctly. :)

## v2.0.0

- `Major overhaul! Reset ALL files from previous versions and start fresh!` Again, old files will NOT work!
- Changes to all aspects of code and files, they are all now prefixed by "AzuAntiCheat_" and are in yaml format.
- Move moderator permissions away from default configuration file and into AzuAntiCheat_ModeratorList.yml
- Moderator perms are now able to be configured per moderator
- Hash checking and simplified files
- Localization added to some messages, more to come! (Localization files are in the format of AzuAntiCheat.Language.yml)
  . Localization files will be found if they are anywhere inside of the plugins folder.
- Webhooks can now be named so you can tell them apart, if you are using more than one.
- All limit checks can now be configured in the AzuAntiCheat.cfg file found on the server
- Instant ban option added if a cheat is detected. Does not instant ban for mismatched mods, since most admins tend to
  mess this up.

## v1.6.0

- Compile against latest version of the game, Update BepInEx/ServerSync.

## v1.5.0

- Important Internal changes.

## v1.4.1 (Quality of life update)

- Show Server name above world name in discord output.
- SteamID section in discord output name changed to Steam Information. It will now include SteamAccountName and SteamID
- Fixed some discord output randomly saying the world name for PlayerLocation
- Additional checks when using Multiverse mod.

## v1.4.0

- ***MAJOR INTERNAL CODE REWORK*** - Please **PLEASE** regenerate your whitelist, greylist, etc files. They now only
  look at loaded plugins (and more efficiently) and does not load all DLLs found in the folder. If you do not heed this
  warning, you will have a lot of false positives for cheating!!!
- Internal GreyList Updates/Fixes. This should help eliminate some issues users were having.
- Reminder, do not have dlls and BepInEx plugin names on the whitelist AND the greylist. Whitelist is only for mods you
  want to enforce on the client, the greylist is for additional mods found on the client that you don't care if they
  have. Some servers were doing this, and it would give blank results on "DLLs Missing"

## v1.3.0

- "Grey List" addition. Put your optional mods in "aac_greyList.txt"
- Comments in the text file starting with "//" shouldn't matter anymore. Left the comments in there to remove it just in
  case there are issues.

## v1.2.8

- Serverside Simulations Damage fix. Heavily tested with and without SSS. We should be good now :)

## v1.2.7

- Serverside Simulations fix
- Bug fix

## v1.2.6

- Fix for killing yourself causing a kick from the server

## v1.2.5

- Bug fixes

## v1.2.4

- Hearth & Home Update/Compatibility

## v1.2.3

- Fix console check issue with certain servers using Better Continents and CLLC with console enabled.

## v1.2.2

- Fix admin check for whitelist on serverside

## v1.2.1

- Fix compatibility with MagicOverhaul (again)
- Add more Moderator config options
- Update to the AntiCheat checks
- Whitelist mode will now require clients to have all mods on the whitelist.
- Color code some output to discord.
- Additional logging for DLLs. Client and Server side to help with issues reported.

## v1.2.0

- Fix compatibility with MagicOverhaul
- REMOVED THE NEED TO RUN AS ADMIN
- Update to the AntiCheat checks

## v1.1.0

- Begin adding configuration options (AzuAntiCheat.cfg)
- Remove creation of config folder, files will now be created directly in config folder with "aac_" prefix
- Default to whitelist option, can be changed back. If using whitelist, you must include all DLL and BepInNames
- Generate BepInNames and DLL names to files in BepInEx/AzuAntiCheat/ folder
    - Files will be repopulated each time you load the game
- Fix errors with File not found on System files
- Log to server logs when webhook is null with information that would have been in webhook
- Eliminate need for litJSON dependency.
- Change format of discord output to be embedded message
    - Swapped player id to now be player location, so you know where they were when the cheat occurred
- Custom disconnect codes to provide compatibility with other mods invoking similar methods
- Prevent and penalize user for attempting to use ExploreAll map cheat
- Code cleanup/optimizations and encoding changes to files

***