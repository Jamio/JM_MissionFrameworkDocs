---
title: DLC Checker         
parent: Features
nav_order: 9
layout: default
---

{: .warning }
This DLC checker is a TOOL, not just a script to run in your missions. It contains two separate parts for you to use, with very specific instructions - read them carefully.

# DLC Checker

*Workflows for checking for DLC gear in your mission*

---

## ✅ Purpose

This system has two parts that work in tandem:

1. A system that allows the mission-maker to see at-a-glance which playable units are using gear that requires a DLC.

2. A system that checks a players gear on mission start, and notifies them if they are using gear from a DLC that they do not own.


---

## ⚙️ How It Works

This system comes with an external tool that will allow you to prepare a registry of all the gear in your game that requires a DLC.

There are then two separate systems that work together.

Editor-Based Check
{: .label .label-yellow }

The first system will check all <b>PLAYABLE</b> units for gear that requires a DLC. 

It will prepare a report for the mission-maker that will be displayed in the briefing section. From here, you can see if there are any playable slots using DLC that you didnt intend.

Player-Based Check
{: .label .label-green }

The second system runs when a player joins the mission.

It will gather all the gear that the player is currently using, and will check it against a pre-prepared DLC gear registry.

The script will alert the player if they are using gear that requires a DLC they <b>do not own</b>


{: .warning }
The editor-based check can <b>only be used in singleplayer</b> - this makes sure that the playable slots are inhabited by AI, and the script has a chance to grab their gear. If this script runs in multiplayer, it cannot retrieve loadouts of uninhabited player slots, and therefore will not give you an accurate list of DLC gear.

---

## 🛠️ Mission Maker Usage

DLC-checking is enabled by default, as it is fairly game-breaking if you turn it off.

The two scripts mentioned above will function automatically. However, to allow them to function properly - you must use the included DLC Parser tool.

### Why?

Some mods use DLC models as a base. Which means, in the arsenal, they appear as mods, but actually require DLC for your players to use.

Therefore, to make sure that our DLC checker knows to look for modded gear that requires DLC as well as DLC gear on its own, we have to create our own array of items that require DLC, mod or not.

<b>This should only need to be done ONCE per modlist, or everytime you add a mod that adds gear that requires a DLC. If you are just adding a sound mod, you don't need to create the DLC Gear Regsitry again.</b>

### How to run the tool

This sounds complicated, but it really isn't - trust me - I've automated the whole thing.

Step 1: Load up your game, with all the mods and DLC you will be using.

Step 2: Load up a blank mission in the editor.

Step 3: Go to the toolbar and click `Tools >> Debug Console`, paste the following code into the box and click `Local Exec`

Step 4: Open up a notepad text file, and paste the output from your clipboard into that file. Save it.

Step 5: Go to the framework and go to JM_Framework >> Misc >> DLCParser

Step 6: Drag and drop your .txt file you saved earlier onto the file labelled `convert_dlc_output.bat`

Step 7: You will have generated a file named `DLC_Output_somethingsomething.sqf`, open it, you should see it as a giant array like so:


<img src="/assets/img/dlc_gear_registry.png" alt="dlc gear registry" style="height: 512px; width:1024px;"/>


Step 8: Copy and paste the entirety of that file into `JM_Framework >> Misc >> DLCParser >> dlcGearRegistry.sqf` - replace anything that currently exists in there.

Step 9: That's it! You now have a functional registry of all the DLC-enabled gear currently in your game. The scripts will use this to check for DLC gear, either in the editor or when a player joins.

---

## 📦 Dependencies


- None

---

## 🔁 Related Features

- [Rally Point System](rally.md)

---

## 🧪 Notes & Tips

- Earplug status persists across respawns.
- Works best when players are expected to experience loud sustained sounds (artillery, gunfire, etc.)

---
