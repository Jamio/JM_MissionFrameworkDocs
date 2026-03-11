---
title: Tickets Medevac       
parent: Features
nav_order: 17
layout: default
---

# Tickets Medevac

*Adds a system for respawning based on tickets replenished by player bodybags*

---

## ✅ Purpose

This system gives the team a set pool of tickets, and lets players replenish that pool by bodybagging dead players and bringing them to a specific location - referred to in this module as the "medical post", but that is literally just a title, it can be anywhere.

This is designed to give logistics or air crews a way of contributing to the medical/respawn loop.

Only player bodybags will contribute to the replenishment. AI bodybags are ignored.


---

## ⚙️ How It Works

The mission-maker determines whether the system is active or not.

Players can access the new JTAC menu by selecting the new `Fire Support` ACE interaction node.

- A list of available fire supports is detailed on the left panel.
- An overview targeting map is presented on the right panel.
- To select targets, players must choose the `Select Target` button, and then left click on the opened map to save the coordinates.
- An ingress direction can be selected also.
- Pressing `Transmit` will activate the selected fire support mission.

---

## 🛠️ Mission Maker Usage

The Ticket Medevac system can be enabled in <span style="color: orange; font-weight: bold;">JM_init.sqf</span> by toggling `JM_TicketsMedevac` to true.

The starting pool of tickets, maximum number of tickets, ticket cost per respawn, tickets replenished per bodybag, and other parameters can all be edited too.

An object must be defined under `JM_TicketsDropoffObjects` - this is the variable name of the object that will contain the action players can use to "submit" bodybags.

A marker must be defined under `JM_TicketsZoneMarker` - this is the marker that will be used to mark an area in which bodybags will be considered "submitted" when the above action is triggered. The radius of this zone can also be altered under `JM_TicketsZoneRadius`.

---

## 📦 Dependencies


- CBA_A3
- ACE

---

## 🔁 Related Features

- [Rally Point System](rally.md)

---

## 🧪 Notes & Tips

- If players lose track of bodies/bodybags, it would be quite easy for them to run out of tickets with no way to replenish them. Consider balancing the pool/replenishment values to adjust this to your liking.

---
