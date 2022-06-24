# Tools

{% hint style="info" %}
**BASED ON:** Sigourn @ [https://github.com/Sigourn/nerevarrising/blob/master/setup.md](https://github.com/Sigourn/nerevarrising/blob/master/setup.md)
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
