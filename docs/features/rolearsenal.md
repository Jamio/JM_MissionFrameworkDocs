---
title: Role-Restricted Arsenal        
parent: Features
nav_order: 5
layout: default
---

# Role-Restricted Arsenal

*Adds a system to define custom arsenal inventories based on a players role.*

---

## ✅ Purpose

This system gives players a customised arsenal inventory that is specific to the role they are defined as.

For instance, medics could be the only ones to have access to medical gear such as personal aid kits, whereas an ammo bearer role might get access to the larger backpacks.

There is also a pool of general gear that is available to every class - useful for uniforms, watches, compasses etc.


---

## ⚙️ How It Works

The mission-maker determines whether the system is active, and the object to be used as a personal arsenal.

Players can access their role-specific arsenal via a scroll-wheel action on the assigned object.

- Arsenal inventories are compiled from a list of general items, merged with class-specific items.
- This system is compatible with the supply framework, and will populate supply crates based on all the magazines and grenades available to players.
- If persistent loadouts through death are not enabled, player loadouts will be saved when they exit the personal arsenal.

---

## 🛠️ Mission Maker Usage

The Role-Restricted Arsenal system can be enabled in <span style="color: orange; font-weight: bold;">JM_init.sqf</span> by toggling `JM_arsenalRoleRestrict` to true.

Roles, and their specific items can be edited in the `JM_allowedArsenalItems` array in this format:

`JM_allowedArsenalItems = [
[ROLENAME, [LIST OF ITEM CLASSNAMES],
[ROLENAME, [LIST OF ITEM CLASSNAMES]
];`

Any items under the role name "General" will be a common item that every role will be able to access.

To give a player a specific role - place this code in the init of that unit via the editor: `this setVariable ["JM_role", "Medic"];` - replacing "Medic" with your role name (must be an exact match).

---

## 📦 Dependencies


- CBA_A3
- ACE

---

## 🔁 Related Features

- [Rally Point System](rally.md)

---

## 🧪 Notes & Tips

- You will have to manually add magazines to the list of allowed items too, so dont forget them or your players will be useless!
- Make sure to match your role names exactly to the names you have defined in your arsenal list.

---
