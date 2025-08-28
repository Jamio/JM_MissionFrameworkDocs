---
title: Object Caching        
parent: Features
nav_order: 15
layout: default
---

# Unknown Weapons

*Adds a system to manage caching, loading and deleting of local objects to help performance.*

---

## ✅ Purpose

This system is designed to allow for the mass-deletion of local objects, to aid performance during missions.

This is useful for missions with lots of local-only props and objects.

---

## ⚙️ How It Works

Usually, local objects are just that - local to the players machine. This means that deleting them via script or zeus will not remove them from the player. In large scenarios with thousands of objects,
even local-only objects can have an effect on performance.

This system uses variables to "tag" items within layers, which can then be used to delete layers containing local objects, and free up resources once your players no longer nearby.


---

## 🛠️ Mission Maker Usage

The Unknown Weapon system can be enabled in <span style="color: orange; font-weight: bold;">JM_init.sqf</span> by toggling `JM_UnknownWep` to true.

The system will automatically account for weapons in player loadouts OR weapons in the role-restricted arsenal, and exclude them from performance debuffs.

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
