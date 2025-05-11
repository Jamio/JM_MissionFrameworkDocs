---
title: Mission-Maker Checklist
nav_order: 6
has_children: true
layout: default
---

<img src="https://jamio.github.io/JM_MissionFrameworkDocs/docs/assets/playerguide.png" alt="Banner" style="width: 100%; max-height: 300px; object-fit: cover;" />

This is a checklist for mission-makers to run through at the end of mission creation. It aims to cover all of the configurable stuff, and double-check all of the essential systems that need to be in place for a functional mission:

## DESCRIPTION.EXT

- [ ] Upload images for preview, loading screen
- [ ] Give mission loading text and briefing text
- [ ] Give mission a title
- [ ] Give mission an authour

## GENERAL
- [ ] Make sure that there are enough slots for the maximum number of players, even if expect much fewer
- [ ] 

## PLAYER LOADOUTS

- [ ] Verify player loadouts exist EITHER through starting gear OR role-restricted arsenal
- [ ] Verify player loaouts contain suitable magazines for primary weapons, secondary weapon and launchers
- [ ] Verify player loadouts contain at least some access to medical items AND/OR a medic role
- [ ] Verify players have access to radios for TFAR - short AND long-rage where appropriate
- [ ] IF role-restricted arsenal THEN verify that roles are set correctly in JM_Init AND player slot int
- [ ] Verify that platoon leader slot with init exists if necessary
- [ ] Verify that loadouts persist on death if necessary
- [ ] Verify that respawning with loadout EITHER from starting gear OR role-restricted arsenal functions correctly

## FRAMEWORK MISC (WILL DEPEND ON YOUR USE-CASE)

- [ ] USE THE FRAMEWORK COMPOSITION IF POSSIBLE
- [ ] Enable or Disable stamina in JM_Init based on your needs
- [ ] Verify respawn position exists
- [ ] Verify redeployment menu exists and is accessible
- [ ] Verify that unconscious spectator functions correctly if turned on/off
- [ ] Verify briefing content exists and is formatted correctly
- [ ] Verify Garage exists and is accessible, vehicles have appropriate spawn limts, and spawn points have been defined
- [ ] Verify that both crates for Fortify system exist and are usable with blueprint lists defined in JM_Init
- [ ] Verify that designated safezones function correctly
- [ ] Verify that non-scalable markers function correctly
- [ ] Set up end titles for cinematic and debriefing text

## SERVER-SIDE
- [ ] Test that any custom scripts function with the framework, AND have no locality issues
- [ ] Check FPS through mission areas, and optimise if severe performance impacts
- [ ] 
