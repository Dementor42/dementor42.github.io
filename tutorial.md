---
title: Tutorial
---

# Tutorial

<video controls>
	<source src="/assets/videos/tutorial.webm" type="video/webm">
	<source src="/assets/videos/tutorial.mp4" type="video/mp4">
</video>

[Listen to the track used in the Video on Spotify](https://open.spotify.com/track/5xXB7wVgRmBHoMBmcfEE3C?si=XliSH7R0QC-OycxxY0gc_w)

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
2. Click the **Add bot** button
3. Select **DarkOrbit Pixel Bot** and install it

## Configure the botscript

Select the just installed bot and click on its **Config** tab. Edit the config to meet your needs. Remember that you can donwload the script multiple times and have multiple configurations (eg. for different accounts).

## Run the botscript

If you don't use auto login you need to load darkorbit.com and login manuelly. Use Crtl-C and Crtl-V to copy paste your login credetials into the botfather browser. Typing doesn't work.

Select your bot, then click the **Start bot** button.

## Get support

Follow these steps if something doesn't work as expected:

1. Enable _debug mode_ in your bots settings
2. Try to **run the botscript** again
3. Save/copy the debug log and [ask for help on our Discord]({{ site.discord_link }}) server