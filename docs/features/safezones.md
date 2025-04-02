---
title: Safezones         
parent: Features
nav_order: 4
layout: default
---

# Safezones

*Adds the ability to define custom "Safezones" where shooting and throwing grenades is prohibited.*

---

## ✅ Purpose

This system allows the mission-maker to define specific safezones in which players bullets and grenades will be deleted.

This can be useful in areas designated as a base, to prevent players from accidentally killing eachother, or trolling.


---

## ⚙️ How It Works

Safezones are defined by the mission-maker with a specific radius.

If a player fires their weapon or attempts to throw a grenade, the bullet or grenade will be deleted and will show that player a warning message.


---

## 🛠️ Mission Maker Usage

The Fortify system can be enabled in <span style="color: orange; font-weight: bold;">JM_init.sqf</span> by toggling `JM_Safezone` to true.

An array of markers to use as safezones, as well as the radius of each zone, can be edited in the customisable section.

The message that displays when someone violates the safezone can also be edited in the same section.


---

## 📦 Dependencies


- None

---

## 🔁 Related Features

- [Rally Point System](rally.md)

---

## 🧪 Notes & Tips

- Don't make the radii of the safezones too big if you plan on having combat anywhere near the safezones - otherwise you run the risk of making it so that your players cannot return fire from their defensive position.
- Reserve safezones for HQs/FOBs/Bases where you are sure there will be no action
---
