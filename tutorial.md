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

1. [Download the bot script](#bot-script-download)
2. [Configure the bot script](#bot-configuration)
3. [Run the bot using botfather](#run-the-bot)
4. [Download botfather](#download-botfather)
5. [Install botfather](#install-botfather)
7. [Configure Adobe Flash](#flashplayer-configuration)

## Bot script download

Our DarkOrbit bot script is hosted on GitHub. GitHub is like Dropbox but for code. Additionaly it provides tools such as issue tracking.

You can [download our bot]({{ site.github_link }}) script from GitHub. Just click the **green download button** on their site and then **Download ZIP**. (If you know what git is you can clone the repo likewise).

![Image of the GitHub download button](/assets/images/github_download.png)

## Bot configuration

Next we want to configure the script file. To do so you first have to extract it using a software like [7zip](https://www.7-zip.org/), [winrar](https://www.rarlab.com/) or your systems default archive extraction tool.

Next use a code editor like [Notepad++](https://notepad-plus-plus.org/) or [Visual Studio Code](https://code.visualstudio.com/) to edit the configuration section of the script file. There are lines which look roughly like this:

```javascript
var CONFIG_USE_PET = false;
var CONFIG_MAX_PET_REPAIRS = 20;
var CONFIG_PET_GEAR_TO_USE = "autolooter"; // "autolooter", "collector", "passivemode", "guardmode"
```

Some settings decide whether the bot shall do something or not. Such settings are called _booleans_. Boolean settings are either ``true`` or ``false``.

Using _numbers_ you can decide how often the bot should do something. Keep an eye open: Sometimes those numbers are seconds, sometimes milliseconds (1 seconds = 1000 milliseconds) or something else.

There are also settings which are configured using _text strings_. Look to the right of those settings to see which strings are allowed.

## Run the bot

The bot script is just a set of instructions for botfather. Thus to run the bot script, botfather is required. If you haven't installed botfather yet, read the next sections and come back to this section later.

Open botfather and **click the start button**. A file chooser dialog will appear. Use it to find and **select the bot script**. The bot script will start immediately. If the start fails for some weird reason, try again. If you broke the script with your configuration, fix it first.

![Image of the botfather toolbar](/assets/images/botfather_icons.png)

## Download botfather

Botfather is a software that executes bot scripts. Botfather does all the technical stuff, our bot script just contains bot logic. So our DarkOrbit bot script runs and depends on their software.

Thus you need to [download botfather]({{ site.botfather_link }}) from the official botfather website. Botfather is availabe for **Microsoft Windows** and **Ubuntu Linux**.

## Install botfather

To install botfather just run the downloaded botfather installer. The installation wizard will ask you where you want to install botfather. Remember the location, for some reason they don't create desktop and startmenu shortcuts.

On Linux: you first have to make the installer executable as a program. To do so rightclick the installer, click _Properties_, go to the _Permissions_ tab, there make sure _Allow executing file as program_ is checked.

### Start botfather

Goto botfathers installation folder and run the botfather.exe. Windows might complain that it's software from an unknown source, but that just means to haven't payed Micro$oft yet to get verified.

If software doesn't run you don't have all it's dependencies installed. [Botfathers dependencies]({{ site.botfather_link }}) are listed on it's download page.

On Windows: You need to install the [Visual C++ 2015 Redistributable](https://www.microsoft.com/en-us/download/details.aspx?id=48145) and have the latest windows updates installed.

On Linux: You have to have all required packages installed. On Ubuntu 18.04 you can do so by executing ``sudo apt install qtdeclarative5-dev qtmultimedia5-dev qtscript5-dev libqt5x11extras5-dev libopencv-*`` in the terminal/console.

## Flashplayer configuration

We all know DarkOrbit requires Flash to be installed. Luckily botfathers browser has Flash support, but you need to install and configure Flash manually.

First [download FP for Opera and Chromium - PPAPI](https://get.adobe.com/flashplayer/otherversions/) from the adobe flashplayer website. On Linux: Choose the ``.tar.gz`` archive version.

![Image of Windows Flash download page](/assets/images/flash_windows_download.png)
![Image of Linux Flash download page](/assets/images/flash_linux_download.png)

On Windows: Just install the just downloaded Adobe Flash installer.

On Linux: Extract the contents from the just download ``.tar.gz`` file and put them somewhere where you can find them easily.

Now **start botfather** and open the **Settings** dialog. There go to the **Browser** tab.

On Windows: Check _Use system wide flash installation_ in the _Flash on Windows_ section and **restart botfather**.

On Linux: Select the earlier extracted ``libpepflashplayer.so`` and ``manifest.json`` files using the **Browse...** buttons in the _Flash on Linux_ section.