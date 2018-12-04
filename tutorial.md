---
title: Tutorial
---

# Tutorial

<video controls>
	<source src="/assets/videos/tutorial.webm" type="video/webm">
	<source src="/assets/videos/tutorial.mp4" type="video/mp4">
</video>

[Listen to the track used in the Video on Spotify](https://open.spotify.com/album/2KTdLUOOs5ZrpAN6eoFtIf?si=K6THIiP2SQGm2TN2nOTUeA)

This is a detailed step by step tutorial guiding you trough the download, installation and configuration of required software and the actual bot script.

To eventually run the bot script you need to have a software called botfather. **Botfather is a bot framework** and will be **used to run the DarkOrbit bot script**, which contains the bots logic.

### TL;DR / Table of contents

1. [Install Botfather](#install-botfather)
2. [Download the botscript](#download-the-botscript)
3. [Configure the botscript](#configure-the-botscript)
4. [Run the botscript](#run-the-botscript)
5. [Get support](#get-support)

## Install Botfather

First you need to [download botfather]({{ site.botfather_link }}) from the official website. Botfather is availabe for **Microsoft Windows** and any modern **Linux** distribution.

### Windows installation

1. Download the [botfather installer]({{ site.botfather_link }})
2. Run the the installer (no admin rights required)
3. Click trough the wizard. Done.

### Linux installation

1. Follow the [Flatpak quick setup guide](https://flatpak.org/setup/)
2. Install the [Botfather Flatpak](https://flathub.org/apps/details/io.botfather.Botfather) from Flathub

## Download the botscript

Botfather has an integreded script manager, from wish you can install and update botscripts listed on their website.

1. Open botfather (from the application menu or desktop shortcut)
2. Click the **Start** button and switch to the **Install** tab
3. Select **DarkOrbit Pixel Bot** and install it

## Configure the botscript

Next we want to edit the script files configuration section. One day this will be possible from the botfather GUI, according to their blog. Until then we have to edit the script manuelly.

1. In botfather go back to the **Manage** tab and select the **DarkOrbit Pixel Bot** script
2. Click **Inspect**. This will open the script folder in your file manager.
1. Edit the script using a code editor like [Notepad++](https://notepad-plus-plus.org/) or [Visual Studio Code](https://code.visualstudio.com/).

The configuration is located at the top of the script and looks roughly like this:

```javascript
var CONFIG_USE_PET = false;
var CONFIG_MAX_PET_REPAIRS = 20;
var CONFIG_PET_GEAR_TO_USE = "autolooter"; // "autolooter", "collector", "passivemode", "guardmode"
```

Some settings decide whether the bot shall do something or not. Such settings are called _booleans_. Boolean settings are either ``true`` or ``false``.

Using _numbers_ you can decide how often the bot should do something. Keep an eye open: Sometimes those numbers are seconds, sometimes milliseconds (1 seconds = 1000 milliseconds) or something else.

There are also settings which are configured using _strings_. Look to the right of those settings to see which strings are allowed.

## Run the botscript

**Important:** Open botfathers integrated browser before running the script. On some systems the browser will crash otherwise, which is a known botfather bug.

If you don't use auto login you need to load darkorbit.com and login manuelly. Use Crtl-C and Crtl-V to copy paste your login credetials into the botfather browser. Typing doesn't work.

1. In botfahter click **Start**
2. Select the **DarkOrbit Pixel Bot** script
3. Click **run**. Done.

## Get support

Follow these steps if something doesn't work as expected:

1. Enable _debug mode_ in the botfather settings
2. Try to **run the botscript** again
3. Save/copy the debug log and [ask for help on our Discord]({{ site.discord_link }}) server