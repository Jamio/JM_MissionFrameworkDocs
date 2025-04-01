---
title: Earplugs         
parent: Features
nav_order: 1
layout: default
---

# Earplugs

*Adds an action to all players to use earplugs, reducing sound volume*

---

## ✅ Purpose

This system allows players to use earplugs to reduce loud sounds. Useful for long helicopter rides and sustained firefights.


---

## ⚙️ How It Works

The earplugs work on a toggleable variable. If it returns true, earplugs are classed as active and sound is reduced, and vice versa.

- Actions to add/remove earplugs are added as scroll wheel actions to all players.
- Audio volume is reduced using Arma’s `fadeSound` and `fadeRadio` commands.
- The earplug status is local per player.

---

## 🛠️ Mission Maker Usage

The ability for players to use earplugs can be enabled in <span style="color: orange; font-weight: bold;">JM_init.sqf</span> by toggling `JM_Earplugs` to true.


---

## 📦 Dependencies


- None

---

## 🔁 Related Features

- [Rally Point System](rally.md)
- [Spectator Mode](spectator.md)

---

## 🧪 Notes & Tips

- Earplug status persists across respawns.
- Works best when players are expected to experience loud sustained sounds (artillery, gunfire, etc.)

---


