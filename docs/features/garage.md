---
title: Garage         
parent: Features
nav_order: 12
layout: default
---

# Garage

*Adds a system to allow players to spawn vehicles.*

---

## ✅ Purpose

This system allows players to spawn vehicles from a predefined list.

This can be useful if you want players to have several vehicles available, but also preserve performance.

This can also be useful for manually handling how many of a particular vehicle you want players to have over the course of the mission.


---

## ⚙️ How It Works

The Garage is populated using a predefined list.

Vehicles will spawn on an appropriate position provided by the mission-maker (Jets on a runway, boats in water etc.)

- Vehicles can be spawned as long as they have not reached the maximum limit for the mission.
- Some vehicles do not have a limit, and can be spawned an infinite number of times.
- Spawned vehicles have their inventory cleared, ready for use.

---

## 🛠️ Mission Maker Usage

The garage can be accessed via an addAction on an object - there is one in the framework composition for you to use. The object can be anything.

The list of vehicles available to players can be edited in <span style="color: orange; font-weight: bold;">JM_init.sqf</span> by configuring the `JM_Garage` array to your liking.

The entry for each vehicle should look like so:

| Index        | Parameter          | Description |
|:-------------|:------------------|:------|
| 0           | "B_MBT_01_TUSK_F" | The classname of the vehicle |
| 1           | Merkava  | Display name of the vehicle in the garage  |
| 2           | 3 | Number of spawns before the vehicle becomes unavailable |

To allow spawning, you will need to have designated a particular spawn area for each type of vehicle.

Place down an empty marker and name it `JM_GarageSpawn_Land` or `JM_GarageSpawn_Air` or `JM_GarageSpawn_Sea`. Any vehicles spawned will appear in their appropriate spawn position.


---

## 📦 Dependencies


- CBA_A3
- ACE

---

## 🔁 Related Features

- [Rally Point System](rally.md)

---

## 🧪 Notes & Tips

- This is a system that is mainly designed to replace respawning vehicles, and avoid Zeus having to spawn new things. Its all in the players' hands.


---
