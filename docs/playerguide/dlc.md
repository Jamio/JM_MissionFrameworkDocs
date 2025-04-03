---
title: DLC        
parent: Player Guide
nav_order: 5
layout: default
---

<img src="https://jamio.github.io/JM_MissionFrameworkDocs/docs/assets/dlc.png" alt="Banner" style="width: 100%; max-height: 300px; object-fit: cover;" />

As we all know, Arma 3 has a bunch of DLC both small and large. For the optional DLCs (Apex, Contact, Marksmen, Tanks, Jets, Laws of War etc.), you are still able to join the server even if they are being used in the mission.

However, if you don't own them and end up using vehicles/equipment that require them, you will get an annoying watermark prompt intermittently.

There are also mods that use DLC models as a base, for things like retexturing. In a lot of cases, these mods don't show you that they require DLC, until you use them...

Then you get the watermarks.


## DLC Checker

To try and avoid this, the framework contains a script that is designed to tell both the mission-maker during editing, and you the player when you join the game, whether you are using gear that requires a DLC.

When you join the mission, your gear will be checked for DLC and ownership. If you don't own the DLC required for gear you are using, you will recieve a small pop-up asking you to notify the Zeus.

If possible, try and make a note of what it is that needs changing in your loadout so that Zeus can easily fix it.

{: .info }
The mission-maker should have already notified you of any slots that require optional DLC. But this check when you start the mission acts as a bit of a backup.


## cDLC Compatibility Mods

On the workshop, there are several mods that allow non-cDLC owners to join the server, even when one or more of the cDLCs are being used in the mission.

These will let you play a mission without owning a cDLC, but will not let you play on the DLC terrain or use the vehicles/equipment.

For instance, if the server was running a mission on Altis, but using some SOG PF assets - by downloading the compatibility mod, you would be able to join. However, you would be locked out of flying the jets, driving the tanks, or accessing SOG PF weapons and gear. You would have to use vanilla gear, or gear from mods entirely.

If, however, the mission was running on Cam Lao Nam - the SOG PF terrain - you would not be able to join in, even with the SOG PF compatibility mod.

It's worth understanding how this works for yours and the mission-maker's sanity, or better yet, commit to getting the DLCs!

