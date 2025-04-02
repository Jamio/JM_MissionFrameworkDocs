---
title: Custom End Mission         
parent: Features
nav_order: 10
layout: default
---

# Custom End Mission

*Allows the the running of a custom end mission cinematic*

---

## ✅ Purpose

This system gives mission-makers an easy to use way of setting up a simple cinematic at the end of the mission.

The cinematic includes a static camera angle, fading text, and finally an end of mission card.


---

## ⚙️ How It Works

The cinematic is called via script or zeus module. This places all players in an <i>end of game state</i> and runs the cinematic locally for everyone.

The cinematic can include text and music.

- Players are healed and placed into captive mode whilst the cinematic runs.
- Camera placement, text and music can be changed by the mission-maker.
- Running this script will actually end the mission once it finishes.

---

## 🛠️ Mission Maker Usage

The custom end mission cinematic can be triggered via script or the zeus module.

The script to execute the endMission must be run on every machine, so remoteExec'ing like so is appropriate:

`["JM_Framework\Misc\endMission.sqf"] remoteExec ["execVM", 0, true];`

Currently, the end mission cinematic is only editable by going into `JM_Framework >> Misc >> endMission.sqf` and customising it.


---

## 📦 Dependencies


- None

---

## 🔁 Related Features

- [Rally Point System](rally.md)

---

## 🧪 Notes & Tips

- The script itself is a bit barebones if you dont know what you're doing with it - I plan on giving it some proper customisability in the configuration file later on.

---
