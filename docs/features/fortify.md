---
title: Fortify         
parent: Features
nav_order: 2
layout: default
---

# Fortify

*Adds a custom ACE Fortify system that allows players to build fortifications and structures using a replenishable budget.*

---

## ✅ Purpose

This system gives players an immersive way to manage building defensive positions using a budet-based and object-based script that utilises the ACE Fortify Framework.


---

## ⚙️ How It Works

A construction object, and a budget are defined by the mission maker. When in a set radius of the construction object, players can access the ACE Fortify menu.

The budget can be replenished by bringing the construction object back to a designated refill object.

Players can also switch between different sets of structures to build by interacting with the construction object.

- Actions to build and replenish are built into the ACE menus.
- Objects and Budgets are fully defined by the mission-maker.
- Budgets can be replenished via specific object to give the impression of having to do "supply runs" to keep the budget or "building supplies" topped up.

---

## 🛠️ Mission Maker Usage

The Fortify system can be enabled in <span style="color: orange; font-weight: bold;">JM_init.sqf</span> by toggling `JM_Fortify` to true.

The objects required to allow building, the budget and the list of structures can all be edited in the customisable section.


---

## 📦 Dependencies


- CBA_A3
- ACE

---

## 🔁 Related Features

- [Rally Point System](rally.md)

---

## 🧪 Notes & Tips

- If you want players to have to go back and forth to replenish, try experimenting with a lower budget than usual.
- If you add too many objects to the lists, they may become extremely cluttered. try not to go overboard with it.

---


