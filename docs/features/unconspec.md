---
title: Unconscious Spectator         
parent: Features
nav_order: 14
layout: default
---

# ACE Unconscious Spectator

*Adds the ability for players to enter a limited spectator mode upon entering the ACE Unconscious state*

---

## ✅ Purpose

This system allows players to view themselves and teamamtes via spectator when they are knocked unconscious using ACE.

This is a good way of making sure that players who are bullet-magnets dont get very bored staring at a completely black screen for long stints.


---

## ⚙️ How It Works

The system intercepts the usual ACE unconscious script, and forces anyone in it into ACE Spectator, limited to their own body and that of teammates.

- The system includes animations that play whilst the player is knocked out.
- The system also includes voice lines that play while the player is down to alert others to their state.
- The system should exclude Zeus and Zeus-controlled units from spectator.

---

## 🛠️ Mission Maker Usage

The Unconscious Spectator system can be enabled in <span style="color: orange; font-weight: bold;">JM_init.sqf</span> by setting `JM_UnconSpectator` to true.

The rest of the scripting is automatic, so there is not much else to set.

There is a variation built into the script that would remove the black screen from the ACE unconscious state, and let players talk, but it is a bit half-finished right now.

At some point in the future I would also like to add the ability to turn on/off the medic callouts.


---

## 📦 Dependencies


- None

---

## 🔁 Related Features

- [Rally Point System](rally.md)

---

## 🧪 Notes & Tips

- You can change the headings to whatever you need, and add as many as you see fit.
- Id recommend keeping the briefing content short and snappy - most people wont read it...

---
