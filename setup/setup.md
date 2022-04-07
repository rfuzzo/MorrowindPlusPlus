# Setup

{% hint style="info" %}
**BASED ON:** Sigourn @ [https://github.com/Sigourn/nerevarrising/blob/master/setup.md](https://github.com/Sigourn/nerevarrising/blob/master/setup.md)
{% endhint %}

## Requirements

* An english copy of the game from [**GOG**](https://www.gog.com/game/the\_elder\_scrolls\_iii\_morrowind\_goty\_edition?gclid=EAIaIQobChMIoaWD-6LP6AIVCxCRCh2a5gPiEAAYASAAEgIUSvD\_BwE).
  * Installation instructions are found on the next section.
* A [**Nexus**](https://users.nexusmods.com/register) account. This guide assumes you are using a Free account, so no need to pay for Premium.
* A file archiver. I recommend [**7-Zip**](https://www.7-zip.org).
* A text editor. I recommend [**Notepad++**](https://notepad-plus-plus.org/downloads/v7.9.5/).
* [**.NET 6 Runtime**](https://dotnet.microsoft.com/en-us/download) (for TES3Merge, a conflict resolution tool).

{% hint style="warning" %}
Users have reported issues with Mod Organizer 2 when using the Steam release of the game, which is why it is not supported by this guide.
{% endhint %}

## Installation

You should install Morrowind outside all default Windows folders (Program Files, Program Files (x86), Desktop, and Documents for example). Windows User Account Control monitors these folders, which can cause problems later on.

Your Morrowind **Root** folder is where Morrowind will be installed, and where the game's executable (**Morrowind.exe**), launcher (**Morrowind Launcher.exe**), and **Data Files** folder will be found.

By default, GOG will install Morrowind to the next directory:

```text
C:\Games
```

This will create a folder in the following path, which we will refer to as our **Root** folder.

```text
C:\Games\Morrowind
```

Additional, you will need a folder where to install our mod manager and keep your mods. I recommend the following path:

```text
C:\Games\MorrowindPlusPlus
```

{% hint style="warning" %}
Make sure you don't create your Morrowind Root folder inside your Morrowind folder. Mod Organizer 2 will fail to register your installed mods.
{% endhint %}

### Cleaning up your GOG installation

The GOG release of Morrowind shipped with files that are of no use to the average player. These files are not necessary and do nothing but clutter up your installation. Some of the files we will delete are the official plugins Bethesda released for Morrowind. These are to be considered low quality mods, with some having received a rework from fans to make them actually worth your while. [**You can read about the official plugins here.**](https://en.uesp.net/wiki/Morrowind:Plugins)

All said, delete the following from your `Morrowind\Data Files` folder in order to free about 700 MBs from your install:

* The **BookArt**, **Icons**, **Meshes**, and **Textures** folders.
* All **.esp** files. There should be 8 of them, corresponding to the 8 official plugins.
* All **.txt** files. There should be 8 of them, corresponding to the 8 official plugins.

Your Data Files folder should now look like this.

![Screenshot](https://raw.githubusercontent.com/Sigourn/nerevarrising/master/pictures/Data_Files.png)
