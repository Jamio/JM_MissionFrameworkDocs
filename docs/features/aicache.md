---
title: AI Caching        
parent: Features
nav_order: 15
layout: default
---

# AI Caching

*Adds a system to cache, load and unload AI units to aid performance.*

---

## ✅ Purpose

This system is designed as a simple means of caching pre-placed AI units, thereby freeing up resources until they are needed.

This is good for missions with lots of pre-placed AI that if left to their own devices, will kill your players' and the servers performance.


---

## ⚙️ How It Works

The system will scan all existing units of a specified side, and both hide AND disable their simulations - essentially rendering them inactive.

When players stray into the predefined distance, the AI will be unhidden and have their simulation enabled - activating them, ready for combat.

From this point on, the games standard dynamic simulation setting take over - meaning that if players stray too far away, the units will be unsimmed until they return.


---

## 🛠️ Mission Maker Usage

The AI caching system can be enabled in <span style="color: orange; font-weight: bold;">JM_init.sqf</span> by toggling `JM_optimiseAI` to true.

There are also two configurable variables for the distance at which the AI should activate, and the sides of AI that should be cached.

The system will handle the caching automatically upon mission start.

If you find that a weapon is accidentally missing from the arsenal/loadouts mid-mission, you can call the following script as a zeus or admin, and it will add that weapon to the whitelist: `["diwako_unknownwp_addWeapon", ["weaponClassName"]] call CBA_fnc_serverEvent;`


---

## 📦 Dependencies


- None

---

## 🔁 Related Features

- [Rally Point System](rally.md)

---

## 🧪 Notes & Tips

- With the role-restricted arsenal enabled - even weapons your players start with will NOT be excluded, so if you are going to use that system - just keep all the weapons as part of the arsenal, and spawn your players empty-handed.

---
