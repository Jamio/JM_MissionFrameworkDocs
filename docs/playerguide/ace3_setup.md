---
title: ACE3 Setup       
parent: ACE3
nav_order: 7
layout: default
---

<img src="https://jamio.github.io/JM_MissionFrameworkDocs/docs/assets/ace3.png" alt="Banner" style="width: 100%; max-height: 300px; object-fit: cover;" />

## Interaction Menu

ACE has its own interaction system, and nearly everything related to ACE revolves around this system.

To interact with objects in front of you, press and hold the windows key. To interact with yourself, hold Ctrl + Windows Key.

From this menu, you can select an option by highlighting it and releasing the menu.

A lot of vanilla interactions are replaced by ACE, so if youre having issues with something, try using the ACE interaction menu first.

## Rebinding Grenades

Because of how close the default medical menu keybind ("H") is to the grenade throw keybind ("G") - there is a high probability of you sausage-fingering the grenade button,
and killing everyone around you. A quick fix is to rebind the grenade throw:

In-game, go to `Options >> Controls >> Weapons` then edit `Throw` and set it to 2x "G" presses. Press OK to save your changes.

## Static Interaction Menus

By default, the ACE Interaction Menu is radial and can move around on screen. This can be really annoying when you're trying to pick a specific option. To help this, we can make tha ACE menu into static lists that are much easier to browse.

In-game, go to `Options >> Addon Options >> ACE Interaction Menu` and enable `Always Display Cursor` and `Display Interaction Menus as Lists`.

Much of this is personal preference at the end of the day, but these are settings that I would definitely recommend changing.


## ACE Pointing

The default game has a keybind to "Ping" like in HLL that will appear for everyone on your team. On the server, this is disabled by default as its messy and not very realistic.

To replace it, we can use ACEs pointing system:

In-game go to `Options >> Controls >> Configure Addons >> ACE Common` and assign the `Action "point finger at"` to ("Shift + T").

Then, in-game when you press Shift + T, your character will point towards an area, which will be marked on-screen for all nearby players.


## ACE View Distance Limiter

<strong>This setting is redundant if we are using a separate view distance mod, which is likely the case</strong>

ACE also has a view distance setting panel that allows you to set variable view distances depending on whether you're on foot, in a ground vehicle or an aircraft.

To configure this for yourself, go to `Options >> Configure >> Configure Addons >> Client >> ACE View Distance Limiter` and set your preferred view distances.


## ACE Volume

Whilst you can still control your games default volume through the audio options, the game can sometimes still be extremely loud. This is particularly true for the transition from vehicles to infantry and vice versa.

ACE has a setting that lets you lower the volume in vehicles.

You can configure this in ``Options >> Configure >> Configure Addons >> Client >> ACE Volume`
