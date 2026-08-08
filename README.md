# Squd Size Mod

![Mod Version](https://img.shields.io/badge/Mod%20Version-v2.0.2-blue)
![Game Version](https://img.shields.io/badge/Phantom%20Brigade-%3E%3D%20v2.0-green)
![Language](https://img.shields.io/badge/Language-YAML-informational)

| Metadata                 | Details                                                      |
|:-------------------------|:-------------------------------------------------------------|
| **Update Date**          | TBD                                                          |
| **Mod Version**          | `v2.0.2`                                                     |
| **Repository**           | [PB.squadSize](https://github.com/miketan-dev/PB.squadSize6) |
| **Programming Language** | YAML                                                         |
| **Minimum Game Version** | v2.0+                                                        |
| **License**              | BSD-3 Clause License                                         |
---

## CREDITS

- Harmony Framework for the patching;
- Phantom Brigade Modding System;
- Brace Yourself Games for the awesome game!

---

## MOD STATUS & DL LINK(S)

- [Steam Workshop](https://steamcommunity.com/sharedfiles/filedetails/?id=3618986473) - [6 Mechs ver.]
- [Steam Workshop](https://steamcommunity.com/sharedfiles/filedetails/?id=3618986072) - [5 Mechs ver.]

- [Nexus Mod](https://www.nexusmods.com/phantombrigade/mods/69) - [Both versions]

---

## INSTALLATION (EPIC GAME VERSION)

To install the mod:

1. Extract the mod folder into the following directory:
   <br>```[Drive]:\Users\[yourUser]\AppData\Local\PhantomBrigade\Mods```
   <br><br>
2. Launch the game; the mod will be automatically detected and activated.

> ⚠️ **[DISCLAIMER]** ⚠️
> <br>While the mod has been fully tested by covering most of the use cases, make sure to back up your save file before
> applying the mod to avoid any unintended (and negative) effects.
> <br><br>I will not be held responsible for any misuse of this mod or any damage caused to
> save files.
> <br>The present project repository is made public to adhere
> to [Brace Yourself Games' guidelines](https://braceyourselfgames.com/mod-policy/).<br>
> The mod author certifies that the present Library Code **DOES NOT CONTAIN/EXECUTE** any kind of malware, stating that the mod does not perform any file/folder creation, if any, outside mod's directory.
> <br><br>You are free to use my mod as a dependency for your mod(s) as long as you give
> credits to me.
> <br>The present project is under **BSD-3 License**, available [here](https://github.com/miketan-dev/PB.squadSize6/blob/Master/LICENSE).

---

## Overview

This mod modifies the game's simulation settings and combat scenarios to enable a total squad size of 6 mechs instead of the default 4. This provides players with greater strategic flexibility and the ability to field more varied mech compositions during missions.

## Mechanics

The mod changes the `activeSquadLimit` parameter in the simulation settings from 4 to 6, allowing you to deploy up to 6 mechs in a single squad.

### Pilot Experience Scaling
To maintain game balance with larger squads, the mod implements a pilot experience scaling system for the additional mech slots:

*squadSize5 version*:
- **Slot 1-3**: Standard experience gain (100%)
- **Slot 4**: 50% experience gain
- **Slot 5**: 25% experience gain

*squadSize6 version*:
- **Slot 1-3**: Standard experience gain (100%)
- **Slot 4**: 50% experience gain
- **Slot 5**: 25% experience gain
- **Slot 6**: 10% experience gain

This scaling ensures that while you can field more mechs, pilots in the additional slots will gain experience at a reduced rate, preventing rapid over-leveling.

### Scenario Modifications
The mod updates combat scenario configurations across the game to support the increased squad size. This includes:

- **Generic scenarios**: Assault, assassination, base showdown, break-in, civilian liberation, crawler defense, elimination, intercept, liberation, military demolition, raid, and underground missions
- **Unique scenarios**: Breakthrough stages, capital center, capital outskirts, stronghold, and test range

All modified scenarios have their `entry.squadSize` parameter updated to 6.

## Compatibility & Exclusions

To maintain fair game balance, this mod does not affect specific scenarios where a 6-mech squad would provide an unfair advantage, particularly in early-game content:

### Excluded Scenarios
- **Mountain Base** - The mod does not apply to this location
- **Early-Game & Tutorial Scenarios** - Tutorial missions remain unaffected to preserve the intended learning experience
  - *Note*: Obstager-Wiel and Hedmark missions are NOT excluded and will benefit from the 6-mech squad size
- **Specialized Missions** - Scenarios specifically designed to field only 2 or 3 mechs in a sortie remain unchanged

These exclusions ensure that the mod enhances the mid-to-late game experience without disrupting the carefully balanced early-game progression.