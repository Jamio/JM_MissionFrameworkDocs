---
title: JTAC System        
parent: Features
nav_order: 13
layout: default
---

# JTAC System

*Adds a system to allow specialist players to call in automated CAS and fire support.*

---

## ✅ Purpose

This system gives players a unique ACE interaction, from which a new menu will allow them to target and specify things like artillery and mortar barrages, CAS gun runs and rocket strafes, and even minefield deployments.

This is designed to allow a potentially smaller group of players to still have access to dynamic fire support options, with some level of customisability from the mission-maker, and also using a clean, easy to use interface.


---

## ⚙️ How It Works

The mission-maker determines whether the system is active or not.

Players can access the new JTAC menu by selecting the new `Fire Support` ACE interaction node.

- A list of available fire supports is detailed on the left panel.
- An overview targeting map is presented on the right panel.
- To select targets, players must choose the `Select Target` button, and then left click on the opened map to save the coordinates.
- An ingress direction can be selected also.
- Pressing `Transmit` will activate the selected fire support mission.

---

## 🛠️ Mission Maker Usage

The JTAC system can be enabled in <span style="color: orange; font-weight: bold;">JM_init.sqf</span> by toggling `JM_JTAC` to true.

The background "skin" for the JTAC menu comes in three flavours - ww2, modern and scifi. The intended skin can be selected by editing `JM_JTAC_theme` in the customisable section.

Available fire missions have to be created under the `JM_JTAC_FireMissions` array. Please refer to the examples within the file to set up your own. The fire mission array as a standardised syntax, but the EPD-specific parameters can vary greatly, so be sure to test and verify before using them.

Things like dispersion, number of rounds, delay and time between rounds can usually be edited via the EPD parameters too.

Each fire mission has its own number of uses (capacity) and a cooldown. Set these to prevent players from spamming certain fire supports, and get them to think about when and how to use them effectively.

To give a player the ability to access the JTAC menu, either use `this setVariable ["JM_isJTAC", true];` in the units init, or toggle the variable using the built-in zeus module.

---

## 📦 Dependencies


- CBA_A3
- ACE

---

## 🔁 Related Features

- [Rally Point System](rally.md)

---

## 🧪 Notes & Tips

- This system is built upon Brians EPD JTAC system, and uses lots of the attack code from that script.
- Setting up new fire support missions can be difficult considering all the different parameters you have to take into account. use the basic ones provided and tweak one value at a time to get your desired effect. Avoid editing multiple parameters at once, lest you lose track of what affects what.

---
