---
title: Loadout Persistence         
parent: Features
nav_order: 6
layout: default
---

# Loadout Persistence

*Enables player loadouts to persist through death.*

---

## ✅ Purpose

This system allows players loadouts to be saved upon death, and reapplied upon respawn.

This is useful if you are trying to simulate attrition, as players will not get a fully refreshed loadout whenever they die.

I would recommend using this in missions where you either want players to have to conserve ammo until resupply, or missions where you want players to be in charge of their own resupply runs.


---

## ⚙️ How It Works

The system functions based on a toggleable variable. If enabled, player loadouts will be saved when they are killed.

That same loadout will be reapplied upon respawning.

- Players will not get a fully-refreshed loadout with this system enabled.
- The equipment and inventory inside each piece of equipment will be saved and reapplied, so missing magazines will also be missing upon respawn.

---

## 🛠️ Mission Maker Usage

The persistent loadout function can be enabled in <span style="color: orange; font-weight: bold;">JM_init.sqf</span> by toggling `JM_loadoutPersist` to true.


---

## 📦 Dependencies


- None

---

## 🔁 Related Features

- [Rally Point System](rally.md)

---

## 🧪 Notes & Tips

- Be careful when using this if you need players to carry unique items - if they are dropped and a player dies, it may be difficult/impossible to retrieve them.
- Works best when players are expected to manage their own resupplies, or be careful with their equipment.

---
