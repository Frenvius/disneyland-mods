Sleepover - Total Bed Control
=============================

This mod adds toggleable options for each of the checks for bed use/sleeping, as well as a couple of small useful additions such as ignoring spawnpoint creation and allowing people to bunk together.

Ability to disable/enable:

* Wet check
* Fire check
* Walls/Roof check
* Enemies nearby
* Sleep without setting spawnpoint
* Sleep in a bed that isn't yours
* Sleep in a bed without claiming it
* Sleep any time of day
* Let multiple simultaneous users in one bed (not well-tested)

Known issues/quirks
-------------------
* Sharing a bed does not make them cuddle side-by-side. They will be attached to the bed at the same location, resulting in some clipping.
* Each connected client (and the server) needs to have the mod installed for the "sleep anytime" component to work. If this is causing problems, simply disable it in the mod.
* This mod is incompatible/untested with other mods that significantly alter bed and/or sleep behaviour.

Example
-------
![Sleep in unclaimed beds - https://github.com/timneill/ValheimMods/tree/main/Skald/dist/Sleepover/bed-01.png](https://github.com/timneill/ValheimMods/tree/main/Skald/dist/Sleepover/bed-01.png)

Config
------
| Config name | Description | Values | Default |
| --- | --- | --- | --- |
| `modEnabled` | Whether or not the game should enable extra bed functions. | `Bool` | `True` |
| `enableMultipleBedfellows` | Allow multiple people per bed. | `Bool` | `True` |
| `sleepAnyTime` | Sleep at any time of day (May be buggy. Disable if there are issues.) | `Bool` | `True` |
| `ignoreEnemies` | Ignore nearby enemies when sleeping. | `Bool` | `True` |
| `ignoreExposure` | Ignore roof and wall requirements for beds. Sleep under the stars! | `Bool` | `True` |
| `ignoreFire` | Ignore fire requirement before sleeping. | `Bool` | `True` |
| `ignoreWet` | Ignore wet status when sleeping. | `Bool` | `True` |
| `sleepWithoutSpawnpoint` | Sleep without first setting a spawnpoint. | `Bool` | `True` |
| `sleepWithoutClaiming` | Sleep without first claiming a bed. | `Bool` | `True` |

Any bugs please use the github tracker: https://github.com/timneill/ValheimMods/issues
