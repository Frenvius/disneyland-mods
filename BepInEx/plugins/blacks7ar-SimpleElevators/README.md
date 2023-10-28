># <b># SimpleElevators</b>

A simple mod that adds a small and large elevators, also adds vertical and diagonal platforms. 

<br/>

[![Watch the video](https://i.ibb.co/k43FFyd/ss3.png)](https://www.youtube.com/watch?v=YYg7P0-VV-c)
![](https://i.ibb.co/98dtS4R/ss.png)
![](https://i.ibb.co/VNWmbdd/ss2.png)

<br/>

>## ## Installation (manual)

- extract `SimpleElevators.dll` file to your `BepInEx\Plugins\` folder

<br/>

>## ## Features

- Adds 2 small elevators that can go up and down, wood and black marble variant.
- Adds 4 large elevators that can go up and down, 2 wood and 2 black marble variants.
- Adds 2 two-way elevators that can go up and down with 3 destinations, wood and black marble variant.
- Adds 6 vertical platforms that can move back and forth, wood and black marble variant.
- Adds 6 diagonal platforms that can go up and down diagonaly, wood and black marble variant.
- Uses vanilla building sizes and snappoints so you can integrate them with your builds.. wooden and black marble builds.
- Configurable recipe, speed and automatic triggers.
- Uses ServerSync and built in config watcher.
- Configurable through config file or [Configuration Manager](https://valheim.thunderstore.io/package/Azumatt/Official_BepInEx_ConfigurationManager/)

<br/>

>## ## Changelog
<br/>

v1.1.1
- fixed minor translation issue.
- updated manifest bepinex dependency string.

<details>
<summary><b>Changelog History</b> (<i>click to expand</i>)</summary>
<br/>

v1.1.0
- fixed multiplayer version check issues

v1.0.9
- updated to the latest valheim build (217.22)
- as requested added an activator to the bottom of the small elevators.

v1.0.7
- removed piece manager.
- added german translation (thanks to @BLUBBSON)
- fixed blackmarbles platform shader (snow and rain now properly applies).

v1.0.6
- updated to the latest valheim build (217.14) hilders request.

v1.0.5
- fixed icons visual glitch.

v1.0.4
- added additional triggers for the two-way elevators to call it up when its down below (end points/beams).
- changed two-way elevators triggers to its end points/beams.
- added config option for platforms speed when moving.
- added elevators/platforms size on its description.
- change the size of small elevators to fit exactly like the wood wall piece size.
- added 4 vertical platforms (4x2 and 4x4, wood and black marble).
- added 4 diagonal platforms (4x2 and 4x4, wood and black marble).

v1.0.2
- added automatic triggers to platforms (can be turned off), if a player step on the platform it will automatically move

v1.0.1
- makes platforms unremovable while player is still on it to avoid a serious bug where if the platform got destroyed the player on it will also be destroyed and unrecoverable.
- fixed an nre when a platform got destroyed while you're on it.
- fixed diagonal platforms integrity.

v1.0.0
- first release

</details>