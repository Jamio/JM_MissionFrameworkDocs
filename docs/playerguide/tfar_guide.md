---
title: TFAR Guide        
parent: TFAR
nav_order: 2
layout: default
---

# TFAR Basics

In missions using Task Force Arrowhead Radio (TFAR), your voice and radio comms are simulated for immersion and realism. 

This section explains how radios work, what each one does, and how to use them effectively.


## Short-Range vs Long-Range Radios

> Short-Range Radios
> - Used for intra-squad communciation
> - Range of 500m - 5km
> - ~16 Channels
> - Examples: PRC-343, PRC-152


> Long-Range Radios
> - Used for communication between squads, with pilots, Command, or across larger distances.
> - Range of 5km - 20km
> - ~100+ Channels
> - Examples: PRC-117F


## Radio Setup

Make sure that you have a radio equipped, either in your radio slot (SR) or as a backpack (LR).

Use the `ACE Self-Interaction Menu >> Radios >> (your radio) >> Open` or press <kbd>Ctrl</kbd> + <kbd>P</kbd> to open your short-range radio/ <kbd>Alt</kbd> + <kbd>P</kbd> to open your long-range radio.

You will be brought to a radio interface. I will show you an example using the PRC-152. The layout of your radio may look different, but the functionality will be the same, just hover over the buttons to see what they do:

<div style="text-align: center;">
  <img src="https://jamio.github.io/JM_MissionFrameworkDocs/docs/assets/radio.png" alt="Radio" style="width: 80%; max-width: 960px; height: auto; border: 1px solid #ccc; border-radius: 8px;" />
  <p style="font-size: 0.9rem; color: #666;"><em>The radio interface of an AN/PRC-152 Short-range radio.</em></p>
</div>

> **1** - Volume control. <i>Clicking this will cycle volume in increments of 10.</i>

> **2** - Current channel. <i>Displays the current channel your radio is set to.</i>

> **3** -  Frequency. <i>Displays the current frequency for this channel. Frequency can be typed in here.</i>

> **4** -  Clear Frequency. <i>Will clear the whatever frequency is currently loaded.</i>

> **5** - Set Frequency. <i>After typing in your desired frequency, pressing this will confirm it.</i>

> **6** - Next/Previous channel. <i>Cycles through all available channels.</i>

> **7** - Speakers/Headphones. <i>Cycles between playing the radio to people nearby also or not.</i>

> **8** - Set Additional channel. <i>Allows an additional channel to be set up.</i>

> **9** - Stereo Settings. <i>Cycles through left/right or both headphone sides for playback</i>

To be able to speak to your teammates, you need to configure your radio to be on the same frequency as them. 

We frequently use the preconfigured channels, so the frequencies are already done for you, but you can also set your own custom frequency by typing it in the display and pressing <b>set frequency</b>.

Otherwise, just pick the channel that you need to be on.

### Stereo Settings

Stereo settings on your radio allow you to force the recieving sound into one or both of your ears. This can be very helpful if you have both a long and short-range radio. Splitting them up allows you to manage two incoming streams of chatter.

### Headphones vs Speaker

By clicking the Speakers/Headphones button, you can cycle between playing the radio for yourself vs broadcasting it to all nearby players in hearing range.

This is really only useful for long-range radios that might be giving important information relevant to everyone. Nobody needs to be listening to your squad chat on speaker.

### Additional Channels

By default, you will be able to set up a single frequency on your radio to recieve and transmit from. However, if necessary, you can set up an additional frequency that you can also transmit and recieve on at the same time.

- Pick your primary channel as normal.
- Select the channel you want to recieve/transmit on additionally by using the `Prev Channel/Next Channel` buttons.
- Press the `Set Additional Channels` button to set that channel as your additional.
- Because you will be listening to two channels on the same radio - whilst you have your additional channel on the screen, you can change stereo settings for that channel only.
- Cycle back to your primary channel


## Radio Usage

Once you're happy with how to configure your radio, its time to use it.

In a mission, you can ask for your squad or command channels. Set your radio up as above based on what channels you are supposed to be on.

When you are ready to transmit, you can do the following:

> <kbd>CAPSLOCK</kbd> - Talk on your currently selected SR channel
> <kbd>T</kbd> - Talk on your additional SR channel
> <kbd>Ctrl</kbd> + <kbd>CAPSLOCK</kbd> - Talk on your currently selected LR channel
> <kbd>Ctrl</kbd> + <kbd>T</kbd> - Talk on your additional LR channel


## Vehicle Radios and Intercoms

Many vehicles come equipped with LR radios. Each seat that has access to the vehicles LR radio must be configured separately.

If you configure the LR radio in the pilot seat, then jump into the co-pilot seat, the radio will not be configured.

You can configure the radios through ACE Interaction menu in the same way you would any other LR radio.

## Intercoms

Many vehicles also have an intercom feature which separates the local, non-radio chat into separate internal intercom channels. The intercom channels function just like direct speech, no broadcasting is needed, but they function like a radio, allowing you to hear your crewmates over the sounds of gunfire or loud helicopter engines etc.

This means you can have an intercom for Crew, Passengers, and more.

To select which channel you are speaking in, use the ACE interaction <kbd>WIN</kbd> and select `Intercom Channel`, then select your desired channel.







