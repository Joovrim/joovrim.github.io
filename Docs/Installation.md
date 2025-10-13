---
title: Installation
layout: home
nav_order: 2
---

# Installation

Please follow all of steps below if it is your first time installing this modlist, if you're updating you can [jump straight there](#updating-joovrim).

<br>

# Table Of Contents

- [Installation](#installation)
  - [Preparation](#preparation)
    - [Install Microsoft Visual C++ Redistributable Packages](#install-microsoft-visual-c-redistributable-packages)
    - [Setup your Page File](#setup-your-page-file)
    - [Setup your Shader Cache](#setup-your-shader-cache)
    - [Configuring Steam](#configuring-steam)
    - [Disable Steam Overlay](#disable-steam-overlay)
    - [Set game language to English](#set-game-language-to-english)
    - [Change Steam's Updating Behavior](#change-steams-updating-behavior)
    - [Clean current Skyrim installation](#clean-current-skyrim-installation)
    - [Install Skyrim](#install-skyrim)
    - [Start Skyrim](#start-skyrim)
  - [Get The Wabbajack](#get-the-wabbajack)
  - [Wabbajack](#wabbajack)
  - [Troubleshooting](#troubleshooting)
- [Post-Installation](#post-installation)
  - [Profiles](#profiles)
  - [Stock Game](#stock-game)
  - [Community Shaders](#community-shaders)
  - [Creating a desktop shortcut](#creating-a-desktop-shortcut)
- [Pre-Game Launch](#pre-game-launch)
  - [Now go read the Gameplay Guide](#now-go-read-the-gameplay-guide)
  - [Controller Bindings](#controller-bindings)
- [FAQ \& Common Issues](#faq--common-issues)
  - [My game won't start even after a fresh install!](#my-game-wont-start-even-after-a-fresh-install)
  - [I get an OpenComposite error when launching the game?](#i-get-an-opencomposite-error-when-launching-the-game)
  - [I Crashed!](#i-crashed)
  - [My performance is really bad!](#my-performance-is-really-bad)
  - [Loading takes too long!](#loading-takes-too-long)
  - [Can't find your issue here?](#cant-find-your-issue-here)
- [Updating Joovrim](#updating-joovrim)
- [Uninstalling Joovrim](#uninstalling-joovrim)
- [Thank You's](#thank-yous)

<br>

---

<br>

## Preparation

### Install Microsoft Visual C++ Redistributable Packages

This package is a must as it is needed by MO2 - you may already have it if you've used MO2 before. If you do not have it, you want to download the x64 version under "Visual Studio 2015, 2017 and 2019".

[Download Visual C++ Redistributable Package.](https://docs.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170)

### Setup your Page File
Skyrim modlists need a large amount of memory purely because of the amount of *stuff* in them  This may not be necessary for a modlist of this size, however, for the best experience, you should setup a pagefile of at least **20GB** - yes, even if you have a million GB of RAM. To setup your pagfile;

1. Hold down the *LEFT* Windows key and press **R**
2. Type in `systempropertiesadvanced` in the run box and then press ENTER
3. Under the "Performance" option, click the "Settings..." button
4. Switch to the "Advanced" tab
5. Under "Virtual Memory", click the "Change..." button
6. Uncheck `Automatically manage...` if it's checked
7. Select your *fastest* SSD in the list of drives
8. Check "Custom Size"
9. Set `Initial Size` to 20480
10. Set `Maximum Size` to 40000
    1.  *Note: some people can get by with just 20480 but if you are experiencing crashes definitely raise it to 40000*
11. Press the "Set" button
12. Press OK
13. Press APPLY and then OK
14. Restart your PC to apply the pagefile setting

### Setup your Shader Cache
Driver defaults from NVidia for shader cache size is limited to 4GB. Being this small can lead to rare crashes in heavily modified Skyrim installs. Increasing the shader cache size is done via the NVidia Control Panel. 

*These instructions are NVidia specific.*

1. Open the NVidia Control Panel
2. Head to `Manage 3D Settings`
3. Scroll down in `Global Settings` to find the `Shader Cache Size` option
4. Set the Shader Cache to *at least* 10GB
5. Done

![Shader Cache](/assets/images/ShaderCache.png)

### Disable Steam Overlay
The Steam overlay is known to cause issues for both Skyrim VR and regular Skyrim SE/AE, especially when using ENBs. I recommend you turn it off to be sure that it doesn't interfere in any way and you can do so by heading into Steam, right
clicking on Skyrim SE in your game library and clicking **Properties** > **General** > **Deselect "Enable Steam Overlay while in-game"**.

### Set game language to English
Wabbajack and some/most of the modding tools out there only support English language versions of Skyrim. Setting the language to English in Steam will stop issues like Wabbajack file verification failures when installing. As with disabling the overlay, right click on Skyrim in your game library and click **Properties** > **Language** > **Select English**.

### Change Steam's Updating Behavior
If for some reason Bethesda decide to release an update for Skyrim, everything will probably break. Well, not *everything* but something will definitely break until mods can be updated to suit. To stop this from happening, you need to tell Steam that you only want to update when you tell it to. You can do this by right clicking on Skyrim in your game library and clicking **Properties** > **Updates** > **Change Automatic Updates to "Only update this game when I launch it"**. Whilst you're in here, it's also recommended to disable Steam Cloud too.

### Clean current Skyrim installation
If you have not yet installed Skyrim, you can skip this part.

1. Right click on Skyrim in your game library and click **Properties** > **Local Files** > **Browse**. 
2. Uninstall the game via Steam - right click on Skyrim in your game library and click **Manage** > **Uninstall**.
3. Check the explorer window for any left over files - if there are any, delete them.
4. Open Windows start menu/search and type in `%LOCALAPPDATA%`.
5. Delete the Skyrim folder.
6. Head to `Documents\My Games` and delete the Skyrim folder.

### Install Skyrim
Once you've done the steps above, you can now set Steam to download Skyrim again but ***do not*** install Skyrim to a protected folder, such as `Desktop`, `Downloads` or `Program Files` of any kind. It's best to create a new, dedicated folder for it using the Steam Library function somewhere on the root of your drive such as `C:\SteamLibrary`. A lot of people have a dedicated secondary drive for their games, keeping the OS install separate; using this secondary drive will also work.

### Start Skyrim
That's right - start the game. You need to let the game do its initial start up jobs such as creating registry entries and generating default config files. Once you've gotten to the main menu you can close the game again.

<br>

## Get the wabbajack
download the wabbajack file from the nexusmods page linked at the top of this wiki, extract it wherever you want but remember where you extracted it to.

## Wabbajack
Installing the list is straight forward, Wabbajack will do most of the heavy lifting for you - you only have to tell it where to put stuff. Open wabbajack, click browse and then click install from disk in the top right

![install-from-disk](/assets/images/installfromdisk.png)

it will open a window for you to select your Joovrim.wabbajack file you downloaded and extracted from the nexusmods page.

Set the installation location to a folder on the root of a drive, something like `C:\Joovrim`. Do not install it to one of the protected folders as mentioned earlier. The download location will have likely been filled in for you too - ensure it matches the directory you set for the installation location, or if you have multiple Skyrim modlists installed, use a common download folder - this will stop you from having to redownload common mods across multiple modlists. You may want to move the download folder outside of the installation folder in order to prevent it from getting wiped on reinstallation.

Before you hit **GO**, a quick tip:

*To get the best performance with Wabbajack, it is recommended that you have the install folder for Wabbajack, the modlist folder and the downloads folder on an SSD; ideally the same SSD.* After the installation is complete, you can move the downloads folder to a storage HDD or other storage medium to save space on your game installation drive. It's not recommended to allow your drive to exceed 90% of its storage space used - Windows Explorer will show a red bar under your drive if you do go over 90% so you need to be sure that you have enough space on your installation drive so that you won't exceed this 90% storage level.

Once you have everything set in Wabbajack, hit **GO** and let it do its thing. It might take a while as there is a fair bit to download and the speed of this will depend on your internet performance as well as your CPU in the later stages for hashing and unpacking the downloads.

<br>

## Troubleshooting
If you're having issues with installation, check the [troubleshooting page](/Docs/Troubleshooting.html). 

<br>

---

<br>

# Post-Installation
Almost there but we're not out of the woods yet! After Wabbajack has given you the installation successful screen, you're free to close it. Navigate to the Joovrim installation folder and run MO2 by double-clicking `ModOrganizer.exe`.

***DO NOT UNDER ANY CIRCUMSTANCES RUN LOOT. The load order is exactly as intended out of the box and you do not need to change it.***

<br>

## Profiles
Joovrim may come with additional profiles based on some of Joov's runs. You can choose these profiles when available by clicking on the drop down menu in the top center of MO2. 

<br>

## Stock Game
Joovrim utilises the stock game feature offered by Wabbajack, meaning that Wabbajack will make a local copy of your Skyrim game files during the installation process. This means that your Steam installation of Skyrim is completely untouched, even by files that go in the game folder.

<br>

## Community Shaders
As a note the first time Community Shaders runs it will have to compile shaders, this may take a while and may look like Skyrim is frozen, just be patient. This process will also most likely be repeated any time you change mods in the list.
The Community Shaders Menu can be opened with END and from here you can toggle individual shaders on and off.

<br>

## Creating a desktop shortcut
Nobody wants to be launching their game via multiple clicks, they want to be able to do it from the desktop! This is simple to do - open MO2, ensure **Joovrim** is selected in the dropdown and click the "Shortcut" button. From the small dropdown menu, click "Desktop". Of course, you can always run from inside of MO2 by clicking the "Run" button instead.

![Desktop Shortcut Creation](/assets/images/DesktopShortcut00.png)

Done! You should now have a shortcut on your desktop which you can now run the modlist from. Don't run Skyrim from within Steam as it won't launch MO2's virtual file system to make a modded game instance.

<br>

---

<br>

## DLSS/FSR/XeSS

These can be selected in the Community shaders menu in the upscaling section, remember only Nvidia GPUs can use DLSS

<br>

---

<br>

## Now go read the Gameplay Guide
[Right here](/Docs/Gameplay%20Guide.html)

<br>

## Controller Bindings
[Controller bindings can be found here](/Docs/ControllerBindings.html)

<br>

---

<br>

# FAQ & Common Issues

<br>

## My performance is really bad!
Your CPU or GPU is too weak. Or, you don't have XMP enabled for your RAM.

Try disabling Community shaders and see if that gives you the boost you need.

<br>

## Loading takes too long!
Shouldn't have put the modlist on a HDD - I did warn you earlier in this very readme.

<br>

## I CTD on launch!
Well, that could be a multitude of things. Make sure you Joovrim folder is added to your antivirus exceptions/allow list and try again.

If you have some heavily aggressive antivirus program such as Webroot, Bitdefender etc, get rid of it.

<br>

## Can I add XYZ?
I don't know, can you?

<br>

## Can't find your issue here?

open an issue on the nexus page or search if it has already been posted there

<br>

---

<br>

# Updating Joovrim
When an update is released, please always check the [changelog](/Docs/Changelog.html) first. You may not need to update your modlist but if there is anything that resolves game breaking issues, it'll be noted in the changelog. Backup your saves before you commit to any updates, Wabbajack doesn't usually touch save files, it does has the ability to delete them if it wanted to.

If you have added anything to this modlist at all, Wabbajack will also delete those. You should know how to stop it from doing this if you're going to add stuff to modlists but if you don't, you have to prepend your mod name with `[NoDelete]` - this will make Wabbajack ignore these files. You will need to reinstall these mods and re-sort their load order after an update though, so I hope you kept backup information on where they went in the load order!

All that aside, updates are basically the same as an installation.

<br>

# Uninstalling Joovrim
No fancy uninstallation needed, you can just delete the Joovrim folder and it'll be gone. There'll be no files left inside your Steam installation folder because Joovrim uses the stock game feature of Wabbajack.

<br>

---

<br>

## Thank Yous

<br>

# Neochiken's Thank You's
  * iAmMe for teaching me almost everything I know about wabbajack, you have been an incredible friend and mentor and words cannot express how much the experience being your friend has meant to me.
  * Joov for giving me the opportunity to make this wabbajack and working with me on it even though he is a very busy man.
  * My wife for keeping me sane.
  * You for playing the list and giving it purpose.