# InteractWhileBuilding for Valheim

Allows you to interact with objects in the world while in build mode.

Enables the Use interactions (Default is 'E' on keyboard) for objects like doors, fireplaces, and containers while holding items like the hammer and hoe.

Adjusts the position of the WearNTear GUI element up slightly so that it doesn't overlap with the action text.

The X and Y axis of the element can be adjusted.

## Installation

1. Download and install BepInEx Valheim
2. Download this mod and move the `InteractWhileBuilding.dll` into `<GameLocation>\BepInEx\plugins`
3. Launching the game will generate a config file at `<GameLocation>\BepInEx\config`

## Configuration
```
[Padding for WearNTear GUI]

## Modify the horizontal positioning of the element
# Setting type: Single
# Default value: 0
# Acceptable value range: From -1000 to 1000
X-axis = 0

## Modify the vertical positioning of the element
# Setting type: Single
# Default value: 20
# Acceptable value range: From -1000 to 1000
Y-axis = 20
```

## Changelog
- v1.0.0
	- Add configuration to adjust GUI X,Y positioning
- v0.0.3
	- Bump up WearNTear GUI element
- v0.0.2
	- Update readme
- v0.0.1
	- initial release