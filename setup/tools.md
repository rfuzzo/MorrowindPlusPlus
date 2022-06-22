# Tools

{% hint style="info" %}
**BASED ON:** Sigourn @ [https://github.com/Sigourn/nerevarrising/blob/master/setup.md](https://github.com/Sigourn/nerevarrising/blob/master/setup.md)
{% endhint %}

## Preamble

In order to address a handful of issues with the Morrowind program (Morrowind.exe), and improve the visual fidelity of our game, we will install a number of tools.

{% hint style="info" %}
You can skip this section if you have all the below tools already installed
{% endhint %}

## ⭐ [**Morrowind Code Patch**](https://www.nexusmods.com/morrowind/mods/19510)

Directly patches bugs in the Morrowind program (Morrowind.exe), which cannot otherwise be fixed by editing scripts or data files. It is a must-have utility for anyone who plays Morrowind, and should be the first utility you ever install.

* Manually download **Morrowind Code Patch** (Main files).
* Extract the contents of the file in your Morrowind **Root** folder (**C:\Games\Morrowind**).

## ⭐ [**MCP Skunk Works**](https://www.nexusmods.com/morrowind/mods/26348)

Repository for the Beta update for the Morrowind Code Patch. Despite being a beta, the patch is perfectly stable and no crashes have been reported from my end or other users of the guide.

* Manually download **MCP beta** (Update files).
* Extract the contents of the file in your Morrowind **Root** folder (**C:\Games\Morrowind**), and overwrite when prompted.

### Morrowind Code Patch setup

* Execute **Morrowind Code Patch.exe**, found in your **Root** folder.
* The **Morrowind Code Patch** will prompt you to install your patches of choice. Use this [**spreadsheet**](https://docs.google.com/spreadsheets/d/1r6fv59to4-KgHJgCm-GDNnwSmD3LdDmamSDEs5jKFdM/edit?usp=sharing) as a reference to install or skip patches.
* Click **Apply chosen patches** when you are finished. Close the application.

{% hint style="info" %}
A backup of **Morrowind.exe** (pre-patch) will apear in your **Root** folder, named **Morrowind.Original.exe**.
{% endhint %}

## ⭐ [**MGE XE**](https://www.nexusmods.com/morrowind/mods/41102?)

The Morrowind Graphics Extender XE allows Morrowind to render distant views, scenery shadows, high quality shaders and other features. MGE XE supports and includes the latest **MWSE 2.1 beta**, so that the newest Lua-based mods work straight away.

* Manually download **MGE XE Installer** (Main files).
* Extract the contents of the file and run the **MGE XE Installer.exe**.
* When prompted to choose an install location, choose your **Root** folder (**C:\Games\Morrowind**).
* When installation has finished, uncheck both options and click **Finish**.
* Go to your **Morrowind\Data Files** folder and delete **XE Sky Variations.esp**.

{% hint style="info" %}
**XE Sky Variations** is an optional mod included in MGE XE that will randomize the sky colour and sunrise/sunset every day. It requires high quality sky scattering enabled (more on that later) and MWSE to be installed. However, a more modern alternative in the form of **Weather Adjuster**, a mod we will install further ahead, is available.
{% endhint %}

Because Morrowind wasn't designed with distant land in mind, certain in-game scenarios which affect the landscape of Morrowind can cause annoying visual issues in the form of pop-ins or fade outs. **Distant static overrides** tell MGE XE to ignore standard distant land generation rules in order to account for these scenarios.

[**abot Distant Static Overrides - Necro Edit 2.0**](https://www.dropbox.com/s/j25igx3p0m5bejs/Abot%20Distant%20Statics%20Override%20-%20Necro%20Edit%202.0.7z?dl=1)\
**Necrolesian**'s edit of **abot**'s custom distant static overrides, which accounts for different stages of the Morrowind and Bloodmoon main quests, as well as certain quests which modify the game's landscape.

* Extract the contents of the file.
* Place the contents of the **necro\_distant\_statics\_override** folder in your **Morrowind\mge3** directory, overwriting when prompted.

This file contemplates the following landscape-altering scenarios:

* The completion of the Main Quest.
* The completion of Bloodmoon's Main Quest.
* The progress and completion of Boethiah's Daedric Quest.
* The completion of the Siege at Firemoth official plugin.
* The completion of the construction of each Great House Stronghold.
* The completion of Raven Rock's construction.

{% hint style="info" %}
The **Readme** elaborates on how to use these overrides, so you should definitely give it a read.
{% endhint %}

## ⭐ [**Mlox**](https://github.com/rfuzzo/mlox/releases/latest)

mlox is a tool for analyzing and sorting your Morrowind plugin load order.

* Expand **Assets** and download **mlox.exe**.
* Place `mlox.exe` in **C:\Games\Morrowind**.

## ⭐ [**Wrye Mash**](https://www.nexusmods.com/morrowind/mods/45439)

Used to repair and update saves, update the masters of mods, and to run tes3cmd in order to clean plugins.

* Download and run **Wrye Mash 2019 x64 - Installer** (Main files).
* When prompted to choose an install location, choose your Morrowind **Root** folder (**C:\Games\Morrowind**).
* When installation has finished, uncheck the option and click **Finish**.
* Download **Wrye Mash 2021 - x64 - beta6 - manual installation archive** (Update files).
* Extract the contents of the file in your Morrowind **Root** folder (**C:\Games\Morrowind**), and overwrite when prompted.
* Launch **mash64.exe**, found in your **Morrowind\Mopy** folder.
* Eventually the installation wizard will ask you to fill the following entries:
  * **Morrowind directory**: select your Morrowind **Root** folder (**C:\Games\Morrowind**). A message should state that morrowind.ini and the Data files folder were found.
  * **Mods Installers directory**: select your Morrowind++ folder (**C:\Games\MorrowindPlusPlus**).
* Click **Next** and then click **Finish**.
* Wrye Mash will now launch. Click **Yes** on the pop-up asking you to enable the MWSE 1024 plugin support. Failing to enable this option can cause you to be unable to repair your saves.
* Close the program.

{% hint style="info" %}
The **Mods Installers directory** we left empty above is redundant to us, as we will use Mod Organizer 2 to install our mods. However, assigning a directory is required to install Wrye Mash.
{% endhint %}

### Cleaning plugins

For general dirty records, we use **Wrye Mash**, automatically cleaning them.

* Run Wrye Mash (**mash64**) in Mod Organizer 2.
* In the **Mods** tab, CTRL+left click on the plugin you want to clean.
* With the plugin selected, right-click and click **Clean with tes3cmd**.
* After the process is over, close the window.

## ⭐ [**tes3cmd**](https://github.com/john-moonsugar/tes3cmd/releases/)

Used to clean plugins by automatically deleting identical-to-master records (records that are usually _unintended_ by the author as they do nothing in practice, but which may override _intended_ changes by other mods) and solve a number of conflicts/issues by means of a plugin, **multipatch.esp**.

* Expand **Assets** under "v0.40-pre-release-2 (with trial Windows .exe)" and download **tes3cmd.exe**.
* Place tes3cmd.exe in **C:\Games\Morrowind\Data Files**.

## ⭐ [**TES3Merge**](https://www.nexusmods.com/morrowind/mods/46870)

Used to solve conflicts by merging conflicting records into a separate plugin, **Merged Objects.esp**.

* Extract the contents of the file in `C:\Games\MorrowindPlusPlus\Tools\TES3Merge`.

## ⭐ [**Mod Organizer 2**](https://www.nexusmods.com/skyrimspecialedition/mods/6194)

An excellent mod manager, offering lots of quality of life conveniences that make modding an easy and quick process. The most popular alternative is **Wrye Mash**. However, I’ve found that it isn’t anywhere near as intuitive as Mod Organizer 2 is, which is why we will only use it for the features Mod Organizer 2 lacks.

* Manually download **Mod Organizer 2** (Main files).
* Run the **Mod Organizer 2.exe**.
* When prompted to choose an install location, choose your Morrowind **Mods** folder (`C:\Games\MorrowindPlusPlus\MO2`).
* When installation has finished, uncheck the option and click **Finish**.

{% hint style="info" %}
It is imperative that, from this point on, you always use Mod Organizer 2 to run the game and to launch any tools you need to use. Mod Organizer 2 uses a Virtual Files folder, which is kept separate from your Morrowind installation. Failing to run the game through Mod Organizer 2 will mean the game won't register any of the installed mods.
{% endhint %}

### Mod Organizer 2 initial setup

* Run **ModOrganizer.exe**.
* Mod Organizer 2 will prompt you to **Create a new instance**. Click **Create a portable instance**.
* You will be asked to select a game to manage. Click **Browse...** and select your Morrowind **Root** folder.
* You will be asked to select a folder where data will be stored. The default MO2 folder is fine.
* Click **Next** and then **Finish**. Mod Organizer 2 will now launch.
* From the pop-up called **Register?**, click **Yes**. This will allow Mod Organizer 2 to handle Nexus links.

{% hint style="info" %}
If Mod Organizer 2 prompts you to **Show tutorial?**, click **No**.
{% endhint %}

### Adjusting mod and load order

Your installed mods are listed on the pane to the left. This is the order in which Morrowind loads their assets, with mods closer to the bottom overwriting the assets of mods closer to the top (if conflicting assets are present). We will refer to it as our **mod order**.

Reorganize it to read as follows using drag and drop.

```text
DLC: Tribunal
DLC: Bloodmoon
```

Your plugins are listed on the pane to the right. This is the order in which Morrowind loads their plugins, with plugins closer to the bottom overwriting the records of plugins closer to the top (if conflicting records are present). We will refer to it as our **load order**.

Reorganize it to read as follows using drag and drop.

```text
Morrowind.esm
Tribunal.esm
Bloodmoon.esm
```

{% hint style="info" %}
You can hide unnecessary information in Mod Organizer 2 by right clicking on the headers above the installed mods, and unchecking the tabs you don't want to see. I suggest unchecking everything but the **Conflicts**, **Flags**, and **Priority** boxes. You can also click on the **X** to the bottom right of the **load order** panel, hiding unnecessary background information seen on the pane below.
{% endhint %}

### Setting up Profiles

Mod Organizer 2 has a feature called **Profiles**, which lets you quickly change from one mod setup to another.

* Click the **Configure profiles** ![Profiles](https://raw.githubusercontent.com/Sigourn/nerevarrising/master/MO2/MO_Profiles.png) button.
* Check the following options:
  * [x] Use profile-specific Game INI files.
  * [ ] Use profile-specific Save Games.
  * [ ] Automatic Archive Invalidation.
* With the **Default** profile selected, click **Copy**. Type in **Morrowind++** and click **OK**. Close the window.
* On the **Profile** tab, select the **Morrowind++** profile.

Morrowind++ will be the profile we'll be modding. You can always revert to the **Default** profile to quickly deactivate all installed mods.

### Mod Organizer 2 tips

#### Mod manager download installation

Mods downloaded from Nexus will be instantly added to Mod Organizer 2 when using the **Mod manager download** option. However, you still need to install these mods for them to work in-game.

* In MO2, click on the **Downloads** tab. You can check the download progress for your file there.
* Right-click the downloaded file, and click **Install**.
* Click **OK**.
* The mod will appear in the left pane. To activate the mod, check the box next to it by clicking the box.

When installing a mod, use the name provided for it in the guide's **hyperlink**. For example, the guide lists the following mod's name as **Graphic Herbalism - MWSE and OpenMW Edition**.

![Example](https://raw.githubusercontent.com/Sigourn/nerevarrising/master/MO2/MO_mod.png)

Whenever you install a mod in Mod Organizer 2, the mod manager assigns it a default name, which is either the name of the Nexus page from where it is being downloaded from, or, when manually installing a mod, the name of the file.

#### Multiple files installation

There will be times when you will need to install multiple files from a single mod page. Mod Organizer 2 will prompt you with the following box.

![ModExists](https://raw.githubusercontent.com/Sigourn/nerevarrising/master/MO2/MO_mod_exists.png)

What these options do is simple:

* **Merge** merges the contents of the file being installed with those of the file of the same name already installed. The new files will take priority over the old files, overwriting as necessary. This option is generally recommended when installing an update file that is separate from the main file, or optional files in the case you don't want to clutter your mod order.
* **Replace** will delete the installed mod, and install the new mod. This option is generally recommended when installing a new version of a mod, as old files may no longer be used by the new version.
* **Rename** will install the mod under a different name, as a separate, additional mod. This option is generally recommended when installing multiple mods from a single mod page that are unrelated to each other (as is the case of compilation pages that list many mini-mods, such as [**Half11's Misc Mods**](https://www.nexusmods.com/morrowind/mods/47068)).

All files installed from a same Nexus page should be merged into a single mod when using Mod Organizer 2. They should also be merged in the order they are listed in this guide, to avoid potential problems (such as update files being overwritten by older files from a same mod). The rule of thumb to use is that one hyperlink in the guide = one single mod on your MO2's left pane.

When the guide asks no specific file to be installed, it is implicit that the file you should download and install is the only main file available for download. Elsewhere, specific instructions will point you in the right direction.

#### Manual download installation

Sometimes authors will block the **Mod manager download** option in Nexus, and you will have to download the mod manually. On occasion, you will download a mod from a different site altogether, be it GitHub, Google Drive, or Morrowind Modding History.

* In MO2, click the **Install a new mod from archive** ![Archive](https://raw.githubusercontent.com/Sigourn/nerevarrising/master/MO2/MO_Archive.png) button.
* Navigate to the folder where the downloaded file is stored and double click on it.

The rest of the steps work exactly as during mod manager download installation.

#### BAIN and FOMOD installers

BAIN and FOMOD installers allow users to customize their install by spliting their mods into multiple options. BAIN installers generally provide a **Core** option which needs to be installed for the mod to work at all, but this option is not always provided, and neither is it always required. FOMOD installers are much more detailed, generally intuitive as opposed to BAIN installers, but sadly these aren't as common in the Morrowind modding scene.

Mod Organizer 2 supports both types of mod installers. Note that this guide will always list the options you should install. If missing, the options should be skipped.

#### Repackaging mods

There will be times you'll be greeted with the following message when installing a mod through Mod Organizer 2.

![InvalidContent](https://raw.githubusercontent.com/Sigourn/nerevarrising/master/MO2/MO_mod_invalid.png)

In lieu of mod authors not fixing their mods themselves, there are two ways to fix this.

* Repackage the mod yourself and install it through Mod Organizer 2.
* Repackage the mod yourself in Mod Organizer 2.

Mod Organizer 2 recognizes anything resembling a valid file structure (having folders such as **Meshes**, **Textures**, **Icons**, etc., or **.esp** and **.esm** files), allowing you to install it.

In the case shown above, the mod contains a **Data Files** folder and a loose **.txt** file acting as the mod's documentation.

* Right-click on **Data Files**.
* Click **Set as data files directory**.
* Click **OK** to install the mod.

![ValidContent](https://raw.githubusercontent.com/Sigourn/nerevarrising/master/MO2/MO_mod_valid.png)

In other cases, mods contain loose assets, and you will have to create folders to package them properly.

* Right-click on the **data files** root directory and click **Create directory...**.
* Enter the name of the folder you want to create, and click **OK**.
* Drag and drop your files in the appropriate folders.
* Click **OK** to install the mod.

#### Hiding files

Mod Organizer 2 lets you hide specific files from your installed mods, be it assets or plugins. A hidden plugin is treated as a deactivated plugin, with the bonus that it will no longer clutter your load order. Hiding assets is useful when you don't want to install specific assets, or when you don't want them to overwrite another mod's.

* Right click on your installed mod and click **Information...**.
* On the **Filetree** tab, right click on the plugins, folders, or files you want to hide, and click **Hide**.
* Mod Organizer 2 will hide the files, and these will no longer affect your game.

#### Overwrite folder

The **Overwrite** folder is the destiny folder for the output of many of the tools we installed in **Setup**, e.g. distant land generation will place its contents inside the **distantland** folder, configurable MWSE mods will place their files inside the **MWSE\config** folder. There's always a chance files in the **Overwrite** folder will overwrite assets and/or plugins from your installed mods.
