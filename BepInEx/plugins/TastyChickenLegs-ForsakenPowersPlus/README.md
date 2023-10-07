# Forsaken Powers Plus

<b>by TastyChickenLegs</b>

This is partly from CakeBlood and RathorDax's ChangeForsakenPowers and Passive Powers mods.  I basically rewrote the entire mod.

Idea credited back to them.

Change the forsaken powers and modify the duration and cooldown.

- Now with ServerSync - ability to turn off version check
- Enable all bosses at once or just the ones you want.
- complied with Mistland’s Final Release 0.212.7
- Complete rewrite of code
- Able to cycle through the forsaken powers to chose which one to use
- Can see all powers or just the one's you have earned
- Can change the durration and cooldown timers
- Can reset current power and startt a new one - even stack powers

```
To Stack Powers do the Following

In the options disable "enable reset"
Hit F and activate your power
HIt F9 to reset the power - Resetting just does not turn off the old power it just allows for a new one.
Hit F8 to cycle through the powers to select a new power
Hit F to start the new power.  They are now stacked as in the image
```

Install the mod into your Bepinex\Plugins and start the game.
Config file will be generated in the Bepinex\Config folder.

|Config Option|Default Value|Definition
|---|---|---|
 |enabledMod |Default True|Enable this mod
 |enabledReset |Default True |Whether or not to enable resetting forsaken power
 |enabledAllBosses |Default False |Whether or not to enable usage of all the bosses or just the ones you have defeated
 |ForsakenPowerHotkey |Default is F8 |Key to Press to cycle between your Forsaken Powers
 |ResetPowerHotkey |Default is f9 |Key to Press to reset the cooldown of your Forsaken Power
 |enableBuffChange |Default is False |Enable changing BuffCooldown and Duration
 |guardianBuffCooldown |Default is 1200 |Boss buff cooldown (seconds) - Game Restart Required
 |guardianBuffDuration |Default is 300 |Boss buff duration (seconds) - Game Restart Required
 |enablepassivemode | Default False| Allows the powers to never run out.  Overrides cooldown and duration timers
 |enableAllBossesAtOnce | Default False| Allows all bosses to be fired at once|       


**Versions**

- 1.3.6

- updated for Valheim 0.271.22


- 1.3.5

Updated to work with Hildir's Request


- 1.3.4

updated to work with newest Valheim Version 216.9

- 1.3.3

no changes updated to newest version of Valheim 0.214.300


-1.3.2

no changes updated to newest version of Valheim


- 1.3.1
no changes.  Version bumpt to match Thunderstore.


- 1.3.0

ServerSync Added for multiplayer
Ownership and player checks added for a reported bug
Version check can be turned on or turned off.  It is by default turned off.

- 1.2.4

update to fix another incompatibility
no other changes.


- 1.2.3

fixed an icompatibility with Monsternomicon
added the queen to the allow all bossses at once setting.


- 1.2.2

fixed toggle through bosses issue
added the ability to turn on all bosses at once.


- 1.2.2

Fixed cycle powers bug

Added ability to activate all powers.

- 1.2.0
 
Fixed The Queen for Mistlands
simplified the configuration
Added a filewatcher so it's no longer necessary to restart the game after making changes


- 1.1.0

Added Passive mode that allows the powers to last forever.  
Stacking powers is allowed so all powers can be on all the time.

- 1.0.0

Initial release built on Valheim 0.212.7 Mistlands Public Release
Complete code rewrite from the original mod changeforsakenpowers
