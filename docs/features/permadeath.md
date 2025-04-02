---
title: Permadeath         
parent: Features
nav_order: 11
layout: default
---

# Permadeath

*Adds a system to prevent respawning whilst enabled.*

---

## ✅ Purpose

This system prevents players from respawning after they die.

It can be useful for missions where you want to control the flow of reinforcements, or maybe dont want people constantly hopping back into the fight straight away.

Nice for building tension and pressure on players without being too punishing.


---

## ⚙️ How It Works

Permadeath sets players respawn timers to infinity - if they die, they just enter spectator.

A function can be called to pull players out of permadeath, and also to toggle permadeath on and off at will.

- Whilst players are dead and permadeath is enabled, they will be notified of that fact.
- Players dead with permadeath enabled will be able to spectate their teammates.
- There are several zeus modules that allow respawning of all or individual players.

---

## 🛠️ Mission Maker Usage

The permadeath system can be enabled in <span style="color: orange; font-weight: bold;">JM_init.sqf</span> by toggling `JM_Permadeath` to true.

Whether permadeath is enabled mid-mission is defined by the public variable `JM_isPermadeathEnabled`

There are zeus modules in the framework that let you toggle permdeath on/off, and handle respawning.


---

## 📦 Dependencies


- CBA_A3
- ACE

---

## 🔁 Related Features

- [Rally Point System](rally.md)

---

## 🧪 Notes & Tips

- Don't forget to respawn people when neccessary - sitting in spectator being dead is not that much fun.


---
