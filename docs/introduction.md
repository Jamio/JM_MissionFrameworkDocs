---
title: Introduction
nav_order: 1
layout: default
---

# 🎮 Jamios Mission Framework

Welcome to the **JM Mission Framework**, a modular system designed to speed up Arma 3 mission development while adding robust features for players and mission makers alike.

---

## 👥 For Players

If you're here to play in a mission using the JM Framework, you don't need to do anything special.

This site mainly serves to give mission-makers the tools to quickly throw together missions, without having to worry about missing pesky respawns or resupplies.

 The framework:

- Enhances immersion with quality-of-life systems (earplugs, spectator view, rally points)
- Handles respawns, unconscious behavior, and supply systems behind the scenes
- Is designed to be invisible unless you're actively interacting with one of its features

As a player, you are ultimately the person who will be affected by things going wrong (or right), so please please please give feedback when you can!

[Player Guide](https://jamio.github.io/JM_MissionFrameworkDocs/docs/playerguide/){: .btn .btn-purple }

---

## 🛠️ For Mission Makers

The JM Framework is a **modular mission framework** designed to be lightweight, readable, and easy to extend.

It includes:
- ✅ **Core systems** (respawn, rally points, unconscious handling, resupplies)
- ✅ **Utility systems** (zeus modules, permadeath system, punishing unknown weapons, marker scaling)
- ✅ **ACE compatibility** is built into the framework from the start
- ✅ Zeus modules for in-mission control and atmosphere

### 🧱 How it Works

The framework is structured as follows:

- **Modular Scripts:** Each system is in its own folder, and can be easily browsed
- **Initialization:** Toggling features on/off, and editing specific features is all handled through `JM_init.sqf`. As a mission-maker, you should rarely need to edit any other file.
- **Configuration:** Most systems are tied to global variables, and can be disabled or enabled wholesale depending on what you need.
- **Integration:** Designed for drag-and-drop use into your mission folder. The framework comes with all the scripts you need to get going.

---

## 📚 Getting Started

To start using the framework, simply download the latest release and add it to your mission folder.

> See the [Setup Guide](setup_guide.md) for a complete walkthrough.

---

## 📦 Notes

- The framework is designed for PvE scenarios. Most systems will not break if used in PvP, but they are not set up to differentiate between two sides, so your mileage may vary.
- It's actively maintained and updated as mission needs evolve
- Feel free to fork or extend the framework — it's meant to be adaptable

---

