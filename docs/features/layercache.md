---
title: Object Caching        
parent: Features
nav_order: 15
layout: default
---

# Layer and Object Caching

*Adds a system to manage caching, loading and deleting of local objects to help performance.*

---

## ✅ Purpose

This system is designed to allow for the mass-deletion of local objects, to aid performance during missions.

This is useful for missions with lots of local-only props and objects.

---

## ⚙️ How It Works

Usually, local objects are just that - local to the players machine. This means that deleting them via script or zeus will not remove them from the player. In large scenarios with thousands of objects, even local-only objects can have an effect on performance.

This system uses variables to "tag" items within layers, which can then be used to delete layers containing local objects, and free up resources once your players no longer nearby.


---

## 🛠️ Mission Maker Usage

The Layer/Object Caching system is enabled by default and runs in the background of the mission when called.

The intended use for this is to group your objects into defined 3DEN layers. Then, select all the objects within a layer and add this to their init: `this setVariable ["JM_layer", "Cleanup2"];` - where "Cleanup2" is the unique name that we will be using to refer to this group of objects.

Then, we can use this "tag" in a function that is called from something like a trigger : `["Cleanup2"] remoteExecCall ["JM_Perf_fnc_delCachedLayer", 0];`

`JM_Perf_fnc_delCachedLayer` will iterate through all objects that have been tagged as Cleanup2 and delete them, on ALL clients even if the objects are local only.

---

## 📦 Dependencies


- None

---

## 🔁 Related Features

- [Rally Point System](rally.md)

---

## 🧪 Notes & Tips

- 

---
