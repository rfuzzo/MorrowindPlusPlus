# Setup

{% hint style="warning" %}
If you're running OpenMW, you can skip all sections labelled with 📃
{% endhint %}

## Requirements

* An english copy of the game.
* A [**Nexus**](https://users.nexusmods.com/register) account. This guide assumes you are using a Free account, so no need to pay for Premium.
* A file archiver. I recommend [**7-Zip**](https://www.7-zip.org).
* A text editor. I recommend [**Notepad++**](https://notepad-plus-plus.org/downloads/v7.9.5/).
* [**.NET 6 Runtime**](https://dotnet.microsoft.com/en-us/download) (for TES3Merge, a conflict resolution tool).

## Installation

{% hint style="warning" %}
You should install Morrowind outside all default Windows folders (Program Files, Program Files (x86), Desktop, and Documents for example). Windows User Account Control monitors these folders, which can cause problems later on.
{% endhint %}

Your Morrowind **Root** folder is where Morrowind will be installed, and where the game's executable (**Morrowind.exe**), launcher (**Morrowind Launcher.exe**), and **Data Files** folder will be found. For example:

```text
C:\Games\Morrowind
```

Additional, you will need a folder where to install our mod manager and keep your mods. For example:

```text
C:\Games\MorrowindPlusPlus
```

{% hint style="warning" %}
Make sure you don't create your Morrowind Root folder inside your Morrowind folder. Mod Organizer 2 will fail to register your installed mods.
{% endhint %}

### Cleaning up your installation

The GOG release of Morrowind shipped with files that are of no use to the average player. These files are not necessary and do nothing but clutter up your installation. Some of the files we will delete are the official plugins Bethesda released for Morrowind. These are to be considered low quality mods, with some having received a rework from fans to make them actually worth your while. [**You can read about the official plugins here.**](https://en.uesp.net/wiki/Morrowind:Plugins)

All said, delete the following from your `Morrowind\Data Files` folder in order to free about 700 MBs from your install:

* The **BookArt**, **Icons**, **Meshes**, and **Textures** folders.
* All **.esp** files. There should be 8 of them, corresponding to the 8 official plugins.
* All **.txt** files. There should be 8 of them, corresponding to the 8 official plugins.

Your Data Files folder should now look like this.

![Screenshot](https://raw.githubusercontent.com/Sigourn/nerevarrising/master/pictures/Data_Files.png)

## ⭐📃 DXVK **[*Original Engine Only*]**

A Vulkan-based translation layer for Direct3D 9/10/11. Gives you more FPS. Yes.

* [dxvk](https://github.com/doitsujin/dxvk/releases/latest)

Install instructions:

* Open the archive with 7zip
* Open the archive within the archive
* Open the x32 folder
* Put the d3d9.dll in that folder into your Morrowind directory

## ⭐📃 [**Morrowind Code Patch**](https://www.nexusmods.com/morrowind/mods/19510) **[*Original Engine Only*]**

Directly patches bugs in the Morrowind program (Morrowind.exe), which cannot otherwise be fixed by editing scripts or data files. It is a must-have utility for anyone who plays Morrowind, and should be the first utility you ever install.

* Manually download **Morrowind Code Patch** (Main files).
* Extract the contents of the file in your Morrowind **Root** folder (**C:\Games\Morrowind**).

## ⭐📃 [**MCP Skunk Works**](https://www.nexusmods.com/morrowind/mods/26348)

Repository for the Beta update for the Morrowind Code Patch. Despite being a beta, the patch is perfectly stable and no crashes have been reported from my end or other users of the guide.

* Manually download **MCP beta** (Update files).
* Extract the contents of the file in your Morrowind **Root** folder (**C:\Games\Morrowind**), and overwrite when prompted.

## ⭐📃 [**MGE XE**](https://www.nexusmods.com/morrowind/mods/41102?)

The Morrowind Graphics Extender XE allows Morrowind to render distant views, scenery shadows, high quality shaders and other features. MGE XE supports and includes the latest **MWSE 2.1 beta**, so that the newest Lua-based mods work straight away.

* Manually download **MGE XE Installer** (Main files).
* Extract the contents of the file and run the **MGE XE Installer.exe**.
* When prompted to choose an install location, choose your **Root** folder (**C:\Games\Morrowind**).
* When installation has finished, uncheck both options and click **Finish**.

## ✨ OpenMW Installation

{% hint style="warning" %}
TODO
{% endhint %}
