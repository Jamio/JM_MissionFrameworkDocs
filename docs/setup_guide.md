---
title: Setup Guide
nav_order: 2
layout: default
---

# Mission Setup

This guide will give you a quick run through on how to get started using this mission framework.

Requirements:

Subscribe to the mission framework composition on steam: INSERT LINK HERE!!!!

---

## Downloading the Framework

<strong>Step 1:</strong> Click the button below to go the framework github repo.

[JM Mission Framework Github](https://github.com/Jamio/JM_MissionFramework){: .btn .btn-blue }

<strong>Step 2:</strong> On the right hand side of the page, under releases, click on the latest release.

<strong>Step 3:</strong> You will be brought to a page with notes about the latest release. At the bottom of the page, you will see a zip file. Click on it to download the framework.


---

## Using the framework in a mission


<strong>Step 1:</strong> Open up Arma 3 with your modlist (CBA_A3 and ACE3 are hard requirements) and head straight to the editor.

<strong>Step 2:</strong> Pick your terrain, open it, and do `File >> Save As` - save your mission with a memorable name under `MPMissions`. Use underscores instead of spaces to help readability.

<strong>Step 3:</strong> Go to file explorer `My Documents >> Arma 3 / Arma 3 - Other Profiles >> MPMissions` - find your mission folder name. It will be formatted with the mission name then the internal terrain name. You should only see something named `mission.sqm` in there. This is the list of objects/units etc. you have placed in the editor.

{: .info }
Examples of a mission folder: "Operation_Overlord.Altis", "MyTestMission.juju.kalahari", "bigbootylatinas_redux.chernarus"

<strong>Step 4:</strong> Keep that folder open. In a new tab, find the framework.zip you downloaded previously, and unzip it to an empty folder of your choice.

It should look something like this:

<img goes here>

<strong>Step 5:</strong> Copy and Paste the entire contents of the framework file, and paste it into your mission folder.

<strong>Step 6:</strong> Open up your mission in Arma 3 again if you closed it. On the right hand tab of the Editor, go to `Groups >> Empty >> Workshop Compositions` and find the framework composition.

<strong>Step 7:</strong> Drop the composition into your mission - this contains all the objects with their inits set up in advance, so less work for you. You can delete them at will if they are not needed.

---

## Configuration

The framework is designed to be as hands-off as possible, though there will be things you want to have control over.

As a mission-maker you will find all of the configurable pieces within the `JM_Framework >> JM_init.sqf` file.

You may also wish to jump into the description.ext to edit things like the loading image, mission name etc.

Beyond that, everything is running in the background. Check out the individual features tabs to see what they require to work.

---

Thats it! You have a functional mission framework in your Arma 3 mission now. Be sure to click `Save` again to make sure that everything meshes properly.

If you encounter any issues, be sure to open a blank mission after saving, then reopen your mission with the framework. This often helps.


