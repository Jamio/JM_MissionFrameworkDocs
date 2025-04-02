---
title: Marker Scaling         
parent: Features
nav_order: 7
layout: default
---

# Marker Scaling

*Adds an system to prevent certain markers from automatically scaling when players zoom in/out of the map.*

---

## ✅ Purpose

This system allows certain markers to retain their size and scale no matter the level of zoom on the in-game map.

This can be useful if you want to try and make an intricate or complex image via markers on the map.

I came across this script whilst needing to make some "direction of attack" layouts for a WW2 Normandy mission. I hated how, if you weren't at the right level of zoom, everything just broke apart into individual pieces when they should've been connected.


---

## ⚙️ How It Works

The system works on a toggleable variable.

- If a certain marker is defined as non-scalable, it will retain its size at all levels of magnification in the in-game map.

---

## 🛠️ Mission Maker Usage

The ability for markers to be non-scalable can be enabled in <span style="color: orange; font-weight: bold;">JM_init.sqf</span> by toggling `JM_MrkScaling` to true.

Markers that you wish to be non-scalable can have their variables names added to the `JM_scaleMrkrs` array in the customisable section.

---

## 📦 Dependencies


- None

---

## 🔁 Related Features

- [Rally Point System](rally.md)

---

## 🧪 Notes & Tips

- This system is a bit niche, but works nicely if you want large-scale drawings on the map via markers to remain consistent.

---
