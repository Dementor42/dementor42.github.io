---
title: About
---

# About

The "PBDO-BOT" bot script is an **free and opensource** javascript file that anyone can study and modify. It contains the bots logic code telling botfather what to do in which situation.

For example: How to navigation maps, how to collect bonus boxes and repair the ship.

#### What is botfather?

Botfather is a third party bot framework. It deals with all the technical stuff like taking screenshots, image recognition and clicking somewhere. With botfather on can create Android, Browser and Desktop bots. We're using their integrated Chromium browser Api to play DarkOrbit.

------

## Collecting Bonus Boxes

<video controls loop>
	<source src="/assets/videos/v1.webm" type="video/webm">
</video>

Our bot script can collect all kinds of _bonus and event boxes_ efficiently. You just need to configure it to do so. Make sure DarkOrbit runs in **2D mode** and your bot script is configured like this:

```javascript
var CONFIG_COLLECT_LOOT = true; // Works only in 2D mode
var CONFIG_COLLECTOR_TIMEOUT_IN_MS = 200; // Increase to reduce CPU/GPU usage, lower to miss no loot.
```

To increase your earnings from bonus boxes consider **botting on PVP maps**. On PVP maps such as 4-1, 4-2 and 4-3 you **get 50% more** loot from bonus boxes.

Further increase your earnings by **spending Research Points** on the Pilot Sheet Skill Tree. Skills like _Luck I_, _Luck I_ and _Tractor Beam II_ increase the _Uridium and Extra Energy_ earned significantly.

Once you collected enough Uridium, a PET drone might be a good investment. But solely having a PET using the _autolooter-gear_ won't increase your earnings by so much. You really want to buy as much _Salvage Protocols_ as possible to eventually **get 36% more** out of boxes collected by your PET.

## Contributing

There are several ways to support this opensource project. A good start would be to **stop spending money** on payed bots. Instead give some of that money to the DarkOrbit developers. No one wants the game to die, we as players just don't want to spend hours grinding while wasting our lives.

Speaking of time wasted: Consider spending some time on learning to **make bots yourself**. That way you have fun playing a game while learning to code.

**Read the bots code**, improve it and think of new features and implement them. We're happy to see your pull request on GitHub.

Last but not least: **Report bugs** by creating and contributing to issues on GitHub.