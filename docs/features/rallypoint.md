---
title: Rally Point        
parent: Features
nav_order: 12
layout: default
---

# Platoon Rally System

*Adds a rally point system that allows players to teleport to and from squad-level and platoon-level rally points*

---

## ✅ Purpose

This system gives players an immersive way to get back into the action by travelling to and from spawn to a system of rally points.


---

## ⚙️ How It Works

The framework assumes there is a consistent "home spawn" where players will respawn. At this "home spawn", there is an interactable object that will allow players to travel to either the platoon rally, one of the squad rallies, or travel directly to a squadmate.

A <span style="color: orange; font-weight: bold;">Platoon Rally</span> can be placed by any player who is currently the leader of <b>any</b> group.

a <span style="color: orange; font-weight: bold;">Squad Rally</span> can be placed by any player who is has been specifically designated as a Squad Leader.

The ability to teleport to a rally point or squadmate can be enabled or disabled by the mission-maker before or during the mission.

- The teleport to rally or squadmate actions are given as scroll wheel actions in the interactable object at base.
- Teleport to squadmate will teleport the player to a randomly selected teammate. If they are in a vehicle, the player will be teleported into an available passenger seat.
- Players can teleport back to base from the Platoon Rally via an interaction labelled `Retreat`.

---

## 🛠️ Mission Maker Usage

The Fortify system can be enabled in <span style="color: orange; font-weight: bold;">JM_init.sqf</span> by toggling `JM_Rally` to true.

The Framework Composition contains a prebuilt rally system with all of the objects and respective init box code.

There are zeus modules in the framework that allow the enabling or disabling of teleporting.


---

## 📦 Dependencies


- CBA_A3
- ACE

---

## 🔁 Related Features

- [Rally Point System](rallypoint.md)

---

## 🧪 Notes & Tips

- The system assumes that players will always respawn on the "respawn_west" (or equivalent) spawn point. This is where you can place your interactable objects. The base can be an entire FOB, or a 2x2 room if players aren't supposed to explore anywhere.
- Teleporting straight to a squadmate is very powerful. There is currently no check on nearby enemies, so it could throw people right into the thick of it. But its fast, so thats the trade off they have...

---
