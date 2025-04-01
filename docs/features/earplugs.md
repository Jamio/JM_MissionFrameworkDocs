---
title: Earplugs         
parent: Features
nav_order: 1
layout: default
---

# [Feature Name]

*A short one-sentence summary of what this feature does.*

---

## 🎯 Purpose

Explain why this feature exists. What problem does it solve for mission makers or players?

> Example:
> This system allows players to use earplugs to reduce loud sounds during firefights, enhancing immersion and usability.

---

## ⚙️ How It Works

Give a brief technical summary of how it functions in-game.

- When the player presses a certain key or uses an ACE interaction, the earplug effect is applied.
- Audio volume is reduced using Arma’s `fadeSound` command.
- The earplug status is remembered per player.

---

## 🛠️ Mission Maker Usage

Explain what a mission maker needs to know to use or configure this system.

- **Enabled by default?** Yes / No
- **Requires ACE?** Yes / No
- **Can it be toggled?** Yes — via `JM_useEarplugs = false;`
- **Customization:** You can change the volume modifier in `config.sqf`.

---

## 📦 Dependencies

List any required mods or components.

- ACE 3 (for interaction menu)
- CBA_A3 (for keybindings)

---

## 🔁 Related Features

- [Rally Point System](rally.md)
- [Spectator Mode](spectator.md)

---

## 🧪 Notes & Tips

- Earplug status resets on respawn unless manually handled.
- Works best when players are expected to experience loud sustained sounds (artillery, gunfire, etc.)

---


