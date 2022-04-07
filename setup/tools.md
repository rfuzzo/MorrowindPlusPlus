# Tools

{% hint style="info" %}
**BASED ON:** Sigourn @ [https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md)
{% endhint %}

## Preamble

In order to address a handful of issues with the Morrowind program (Morrowind.exe), and improve the visual fidelity of our game, we will install a number of tools.

In addition, we will install a mod manager to help us keep our mods organized, and a series of additional tools to help us fix conflicts between our mods to get our install running as smoothly as possible.

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

## ⭐ [**Mlox**](https://github.com/mlox/mlox/releases/latest)
mlox is a tool for analyzing and sorting your Morrowind plugin load order.

* Expand **Assets** under "It lives: 1.0 Release with an all new GUI" and download **mlox.exe**.
* Place `mlox.exe` in **C:\Games\Morrowind\Data Files**.
* Double click `mlox.exe` and run the program once and close it (do nothing)

## ⭐ [**Mlox Rules**](https://github.com/mlox/mlox/releases/tag/v1.0)
Mlox Rules is a very up-todate rule set sort your plugins and is essential for this modlist to work.

* go to `%localappdata%/mlox/mlox` (type this into windows explorer)
* download all three files from the Mlox Rules repo and save them there:
`mlox_base.txt`, `mlox_user.txt` and `Update_Rules.bat`

## ⭐ [**Wrye Mash**](https://www.nexusmods.com/morrowind/mods/45439)

Used to repair and update saves, update the masters of mods, and to run tes3cmd in order to clean plugins and generate a **multipatch**.

* Download and run **Wrye Mash 2019 x64 - Installer** (Main files).
* When prompted to choose an install location, choose your Morrowind **Root** folder (**C:\Games\Morrowind**).
* When installation has finished, uncheck the option and click **Finish**.
* Download **Wrye Mash 2021 - x64 - beta6 - manual installation archive** (Update files).
* Extract the contents of the file in your Morrowind **Root** folder (**C:\Games\Morrowind**), and overwrite when prompted.
* Launch **mash64.exe**, found in your **Morrowind\Mopy** folder.
* Eventually the installation wizard will ask you to fill the following entries:
  * **Morrowind directory**: select your Morrowind **Root** folder (**C:\Games\Morrowind**). A message should state that morrowind.ini and the Data files folder were found.
  * **Mods Installers directory**: select your Morrowind Sharp folder (**C:\Games\Morrowind Sharp**).
* Click **Next** and then click **Finish**.
* Wrye Mash will now launch. Click **Yes** on the pop-up asking you to enable the MWSE 1024 plugin support. Failing to enable this option can cause you to be unable to repair your saves.
* Close the program.

{% hint style="info" %}
The **Mods Installers directory** we left empty above is redundant to us, as we will use Mod Organizer 2 to install our mods. However, assigning a directory is required to install Wrye Mash.
{% endhint %}

## ⭐ [**tes3cmd**](https://github.com/john-moonsugar/tes3cmd/releases/)

Used to clean plugins by automatically deleting identical-to-master records (records that are usually _unintended_ by the author as they do nothing in practice, but which may override _intended_ changes by other mods) and solve a number of conflicts/issues by means of a plugin, **multipatch.esp**.

* Expand **Assets** under "v0.40-pre-release-2 (with trial Windows .exe)" and download **tes3cmd.exe**.
* Place tes3cmd.exe in **C:\Games\Morrowind\Data Files**.

## ⭐ [**TES3Merge**](https://www.nexusmods.com/morrowind/mods/46870)

Used to solve conflicts by merging conflicting records into a separate plugin, **Merged Objects.esp**.

* Extract the contents of the file in **Morrowind Sharp\Tools\TES3Merge**.

## ⭐ [**Mod Organizer 2**](https://www.nexusmods.com/skyrimspecialedition/mods/6194)

An excellent mod manager, offering lots of quality of life conveniences that make modding an easy and quick process. The most popular alternative is **Wrye Mash**. However, I’ve found that it isn’t anywhere near as intuitive as Mod Organizer 2 is, which is why we will only use it for the features Mod Organizer 2 lacks.

* Manually download **Mod Organizer 2** (Main files).
* Run the **Mod Organizer 2.exe**.
* When prompted to choose an install location, choose your Morrowind **Mods** folder (**C:\Games\Morrowind Sharp\MO2**).
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

```
DLC: Tribunal
DLC: Bloodmoon
```

Your plugins are listed on the pane to the right. This is the order in which Morrowind loads their plugins, with plugins closer to the bottom overwriting the records of plugins closer to the top (if conflicting records are present). We will refer to it as our **load order**.

Reorganize it to read as follows using drag and drop.

```
Morrowind.esm
Tribunal.esm
Bloodmoon.esm
```

{% hint style="info" %}
You can hide unnecessary information in Mod Organizer 2 by right clicking on the headers above the installed mods, and unchecking the tabs you don't want to see. I suggest unchecking everything but the **Conflicts**, **Flags**, and **Priority** boxes. You can also click on the **X** to the bottom right of the **load order** panel, hiding unnecessary background information seen on the pane below.
{% endhint %}

### Adjusting Morrowind.ini

One of the patches we installed with the Morrowind Code Patch, **Rain/snow collision**, requires a few .ini edits to work properly.

* Click the **Tools** ![Tools](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO\_ini.png) button, and click **INI Editor**. **morrowind.ini** will now open.
* Use CTRL+F to input the section names and edit the respective entries to use these values. Note that **Weather Snow** may be found much further down below than the others, just below the **Archives** section.

```
[Weather Rain]
Rain Diameter=1200
Max Raindrops=1500

[Weather Thunderstorm]
Rain Diameter=1200
Max Raindrops=3000

[Weather Snow]
Snow Diameter=1600
Max Snowflakes=1500
```

* Click **Save** and close the window.

### Setting up Profiles

Mod Organizer 2 has a feature called **Profiles**, which lets you quickly change from one mod setup to another.

* Click the **Configure profiles** ![Profiles](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO\_Profiles.png) button.
* Check the following options:
  * [x] Use profile-specific Game INI files.
  * [ ] Use profile-specific Save Games.
  * [ ] Automatic Archive Invalidation.
* With the **Default** profile selected, click **Copy**. Type in **Morrowind Sharp** and click **OK**. Close the window.
* On the **Profile** tab, select the **Morrowind Sharp** profile.

Morrowind Sharp will be the profile we'll be modding. You can always revert to the **Default** profile to quickly deactivate all installed mods.

### Registering tools in Mod Organizer 2

For our modding tools to work in Mod Organizer 2, we need to register and configure them.

Follow these steps for **Wrye Mash**:

* Click the **Modify Executables** ![Executables](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO\_Executables.png) button.
* Click the **Add an executable** ![AddExe](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO2\_Add\_File.png) button and select _Add from file..._.
* Navigate to **C:\Games\Morrowind\Mopy** and double click **mash64.exe**.
* Click **Apply** and then **OK**.

* Click the **Add an executable** ![AddExe](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO2\_Add\_File.png) button and select _Add from file..._.
* Navigate to **C:\Games\Morrowind** and double click **MWSE-Update.exe**.
* Click **Apply**.

* Click the **Add an executable** ![AddExe](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO2\_Add\_File.png) button and select _Add from file..._.
* Navigate to **%localappdata/mlox/mlox%** and double click **Update_Rules.bat**.
* Click **Apply**.

Follow these steps for **MLOX**, **TES3Merge**, **TESAME**, and **TES3View**:

* Click the **Modify Executables** ![Executables](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO\_Executables.png) button.
* Click the **Add an executable** ![AddExe](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MO2\_Add\_File.png) button and select _Add from file..._.
* Navigate to the folder of the tool you want to install (each found inside **C:\Games\Morrowind Sharp**) and double click its .exe file.
* In the **Start In** field, select your Morrowind **Root** folder (**C:\Games\Morrowind**).
* Click **Apply**, and repeat the process for the remaining tools.

{% hint style="info" %}
Unlike the other tools, tes3cmd doesn't need to be registered in Mod Organizer 2 as it is directly run from Wrye Mash, which we have already registered.
{% endhint %}

## Configuring MGE XE in Mod Organizer 2

* In Mod Organizer 2, click on the executables dropdown menu to the left of the **Run** button, and select **MGE XE**.
* Click **Run** to run the executable.

### In-game tab

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MGE%20XE%20In-game%20272.png)

{% hint style="warning" %}
You may be tempted to enable **High detail actor shadows (buggy)**. As the name says, they are buggy and can be very taxing on your framerate. I don't recommend them.
{% endhint %}

### Config tab

* Click the **Report max AA and AF** under **Information** to get your graphics card's max antialiasing and anisotropic filtering levels.

### Graphics tab

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MGE%20XE%20Graphics%20272.png)

Apart from the recommended settings (as seen on the image), there are a couple of options you should look out for.

**Display**

* You should select your resolution and refresh rate.
* Set your **Antialiasing** and **Anisotropic filtering** settings to the values reported in the **Config** tab.
* Turn **VSync** on to prevent screen-tearing.

**Windowed mode**

* Most users then to ALT+TAB during gameplay. However, if you want to maximize performance at the cost of stability when ALT+TABbing, you should uncheck this option.

**Renderer**

* Check **Enable shaders**.
* Higher **Menu UI scaling** settings will scale up the UI. If you are playing on high resolutions (1080p and higher) I recommend starting with values at 1,20.
* Lower **FPS Limiter** settings will increase the consistency of your framerate. I personally set it to **60**.

**Shader setup...**

* On the **Set active shaders** window, click **Modding >>>**. Double clicking on the **Available shaders** makes them **Active shaders**, meaning the game will run them.
* For now, set your shader combination as follows.

```
SSAO HQ
Underwater Effects
Underwater Interior Effects
Sunshafts
```

* Click **Save** after setting up your shader chain.

{% hint style="warning" %}
Note that **Antialiasing**, **Anisotropic filtering**, **VSync**, and **Enable shaders** will all take a heavy toll on your framerate.
{% endhint %}

### Distant Land tab

This tab lets you generate distant land, which in other words means you will see beyond the vanilla Morrowind fog. Tweaking these settings to achieve the optimal look can be difficult, and it boils down to personal taste. Distant Land can really hurt your FPS, especially when used alongside shaders, as there's more to post-process.

All options minus **Use Distant Land** and **Distant land generator wizard** are disabled when you get to this tab. We need to generate distant land for these options to become available.

* Click **Distant land generator wizard**.
* On the **Distant Land Setup Wizard**, click **Select all**. The checked plugins will be used for distant land generation.
* Click **Continue**. This will open the **Distant Land Generation** window.
* In the **Land Textures** tab, simply click **Create Land Textures**. By default, the options you should see are 2048 and 1024 texture and normalmap resolution, respectively.
* In the **Land Meshes** tab, select **Ultra High** from the **World mesh detail** dropdown menu. Click **Create Land Meshes**.
* In the **Statics** tab:
  * Set **Minimum Static Size** to 100.
  * Check **Include reflective water in interiors**.
  * Check **Use lists of statics overriding parameters set above**.
  * Click **Edit list**.
    * Click **Add**.
    * Navigate to your **Morrowind\mge3** folder, and double-click **00\_main.ovr**.
    * Click **Save**.
  * Click **Create Statics**.
* Once the statics have been created, click **Finish**.

{% hint style="info" %}
A rule of thumb is to regenerate your distant land any time you install or uninstall mods. Most importantly, the process will be much easier as you only need to click on **Run above steps using saved / default settings** the next time you are on the **Distant Land Generation** window. On your first distant land generation, MGE XE defaults to **Distant Land configuration setup...**.
{% endhint %}

![Screenshot](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/MGE%20XE%20272.png)

Now that you are back on the **Distant Land** tab you will see all previously unavailable options are now enabled. To get you started, I recommend you copy the settings as shown in the image above. In the future you may want to modify them.

> ℹ️ These draw distance settings will preserve the foggy aesthetic of vanilla Morrowind, which I recommend over the absurd draw distance seen in most modern Morrowind screenshots. If you are aching for a little bit of extra draw distance, I suggest increasing the **Draw Distance** to 5,0, and cranking up the **Above Water Fog** settings to Start 3,0 and End 5,0.

{% hint style="warning" %}
Note that Per-pixel lighting takes a heavy toll on your framerate. You can disable it entirely, or limit it to **Interiors only**.
{% endhint %}
