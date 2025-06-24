---
title: Unknown Weapons        
parent: Features
nav_order: 14
layout: default
---

# Unknown Weapons

*Adds a system to deter players from scavenging enemy weapons unless absolutely necessary.*

---

## ✅ Purpose

This system is designed to deter, but not outright remove, the ability for players to pick up enemy weapons.

This is good for those times when you spend a long time meticulously crafting loadouts, only for everyone to pick up enemy AKs - then they complain about resupply.

This is also a good system to simulate enemy weapon maintenance, or your players' familiarity with enemy weapons systems being poor.

---

## ⚙️ How It Works

Weapons that are not explicitly defined by the mission-maker will have moderate to severe problems with accuracy, jamming, overheating etc.

Friendly weapons are excluded from this, and thus, players are encouraged to stick to their loadouts, putting emphasis on proper resupplies.


If you find that a weapon is accidentally missing from the arsenal/loadouts mid-mission, you can call the following script as a zeus or admin, and it will add that weapon to the whitelist: `["diwako_unknownwp_addWeapon", ["weaponClassName"]] call CBA_fnc_serverEvent;`


---

## 🛠️ Mission Maker Usage

The Unknown Weapon system can be enabled in <span style="color: orange; font-weight: bold;">JM_init.sqf</span> by toggling `JM_UnknownWep` to true.

The system will automatically account for weapons in player loadouts OR weapons in the role-restricted arsenal, and exclude them from performance debuffs.


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
