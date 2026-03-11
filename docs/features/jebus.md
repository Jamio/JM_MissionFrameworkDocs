---
title: JEBUS       
parent: Features
nav_order: 15
layout: default
---

# JEBUS

*JEBUS, or Just Editor Based Unit Spawning, is a robust system for handling dynamic unit spawning, respawning and caching - this is a slightly modified version of the original produced by DreadPirateAU.*

---

## ✅ Purpose

This system gives mission-makers the ability to pre-place units in th editor and have them cached, but able to respawn and perform things like patrols.

This reduces the level of micromanagement needed from Zeus in the mission. The system is very flexible and can be configured in several ways.


---

## ⚙️ How It Works

The system is active and available at all times through script files.

Mission-makers must pre-configure any JEBUS integration they need prior to the mission starting.

---

## 🛠️ Mission Maker Usage

JEBUS is initialised using lines of code in the init of AI Squad Leaders. There are several configurable parameters to allow respawns, custom waypoints, custom inits, caching and more...

These are the parameters and examples taken from the JEBUS wiki:

`
Parameters:
this				= Leader of a group
"LIVES="			= Number of times group should respawn
				  Integer or array [minLives, maxLives]. Default is infinite lives
"DELAY="			= Delay in seconds before respawning
				  Number or array [minTime, maxTime]
				  Default is 30 seconds
"CACHE="			= Group will cache until players are within "CACHE=" metres
				  Default is no caching
"REDUCE="			= Group will cache until players are within "REDUCE=" metres
				  Default is no reducing
"START="			= Initial spawning delay. Use if you spawn multiple groups by one trigger to avoid spawn
				  lag. Default is 0.
"GAIA_MOVE="			= Group added to GAIA with "MOVE" parameter
"GAIA_NOFOLLOW="		= Group added to GAIA with "NOFOLLOW" parameter
"GAIA_FORTIFY="			= Group added to GAIA with "FORTIFY" parameter
"FLYING"			= Air vehicles will spawn already flying
"RESPAWNMARKERS="		= Array of alternate respawn positions
"PAUSE="			= Radius in which enemies will pause the spawner. Default is 0.
"EXIT="				= Name of exit trigger
				  Group will not respawn again once trigger is activated
"INIT="				= Init string to run upon spawning
				  (Use "_proxyThis" where you would usually use "this" in a script or function call)
				  Default is empty string.
"RECRUIT="			= Units in group can be recruited by players
"DEBUG"				= Will provide debugging information

Examples:

0 = [this] spawn jebus_fnc_main;
Respawns group with default parameters. Uses editor waypoints.

0 = [this, "LIVES=", [4,8]] spawn jebus_fnc_main;
Respawns group 4 - 8 times. Uses editor waypoints.

0 = [this, "DELAY=", [30,60]] spawn jebus_fnc_main;
Respawns group after 30 - 60 seconds delay. Uses editor waypoints.

0 = [this, "CACHE=", 500, "GAIA_NOFOLLOW=", "3"] spawn jebus_fnc_main;
Group uncaches when players are within 500m of spawn position. Assigns group to GAIA zone 3.

0 = [this, "PAUSE=", 100, "INIT=", "[_proxyThis, 'agia'] execVM 'UPS.sqf'"] spawn jebus_fnc_main;
Group initializes Kronzky's UPS script to patrol a marker named 'agia'.
Respawning will pause if enemies are within 100m of spawn position.

0 = [this, "GAIA_MOVE=", "9", "RESPAWNMARKERS=", ["m1", "m2"]]spawn jebus_fnc_main;
Group will respawn randomly at its editor position or "m1" or "m2". Assigned to GAIA zone 9.

0 = [this, "GAIA_NOFOLLOW=", "10", "EXIT=", myExitTrigger] spawn jebus_fnc_main;
Group will respawn until myExitTrigger is activated.
`

---

## 📦 Dependencies


- CBA_A3
- ACE

---

## 🔁 Related Features

- [Rally Point System](rally.md)

---

## 🧪 Notes & Tips

- JEBUS is extremely configurable, but make sure to test before doing anything drastic. If this is your first time using JEBUS, I would recommend trying to use it for one or two patrol squads, and see how that fares first before doing anything more advanced.

---
