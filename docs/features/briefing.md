---
title: Custom Briefing         
parent: Features
nav_order: 8
layout: default
---

# Custom Briefing

*Adds a custom, stylised briefing entry*

---

## ✅ Purpose

This system allows mission-makers to prepare a nicely formatted briefing that will appear in the players' vanilla briefing screen.

This is designed in a way to allow it to be easy for mission-makers to add to, without worrying about formatting.


---

## ⚙️ How It Works

The system will prepare a stylised briefing document from a configurable array.

- The system allows coloured text for headings and subheadings.
- Several headings can be used, each leading to their own page of subheadings and corresponding text.

---

## 🛠️ Mission Maker Usage

The custom briefing can be edited in <span style="color: orange; font-weight: bold;">JM_init.sqf</span> by editing the `JM_BriefingContent` array.

The briefing content array must be formatted like so:

`JM_BriefingContent = [
["PAGE NAME", [["SECTION NAME", "SECTION TEXT"], ["SECTION NAME", "SECTION TEXT"]]],
["PAGE NAME", [["SECTION NAME", "SECTION TEXT"], ["SECTION NAME", "SECTION TEXT"]]]
];

The `"PAGE NAME"` is what will appear as a main heading, whilst `"SECTION NAMES"` will help divide the page into subsections.

As many pages and subsections can be added as needed - the script iterates through the whole thing.

The font, colour and size of the text is not immediately configurable, but CAN be configured if you go to JM_Framework >> Misc >> briefing.sqf and change the defines.


---

## 📦 Dependencies


- None

---

## 🔁 Related Features

- [Rally Point System](rally.md)

---

## 🧪 Notes & Tips

- Be VERY careful about the formatting of `JM_BriefingContent` - it is not that user friendly, and is essentially two nested arrays together. If in doubt, copy out one of the example sections and test it by editing the text ONLY.
- You can change the headings to whatever you need, and add as many as you see fit.
- Id recommend keeping the briefing content short and snappy - most people wont read it...

---
