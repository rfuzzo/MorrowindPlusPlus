# Finishing

{% hint style="info" %}
If you're running OpenMW, you can skip all sections labelled with 📃
{% endhint %}

If you just installed this modlist or ar updating it you need to always run the following steps in this order:

## 📃 Memory Management

The game still struggles with the 32bit memory limit the program has. There are a couple of things you can do to aleviate the issue. And make sure you have the mod **Memory Monitor installed**, it will display when the game is about to crash.

### Ini Tweaks

There are some ini tweaks you can do to help with memory:

* Click the **Tools** button, and click **INI Editor**. **morrowind.ini** will now open.
* Use CTRL+F to input the section names and edit the respective entries to use these values.

```text
Interior Cell Buffer=0
Exterior Cell Buffer=0

DontThreadLoad=0
```

### External Programs

* You may configure an exception in your Anti-Virus program for the Morrowind directory
* Close overlays or programs like RivaTuner Statistics Server before starting Morrowind if you have memory proplems while in game

{% hint style="info" %}
{% endhint %}

## 📃 01 Updates

* Run **MWSE-Update** from your game folder.

## 02 MLOX

* Run **MLOX** in Mod Organizer 2.
* Wait for it to load
* Check the **Status** and **Messages** Tabs for errors or incompatibilities
* Click **Update Load Order**
* Close the Window.

## 03 Cleaning plugins

* Run Wrye Mash (**mash64**) in Mod Organizer 2.
* In the **Mods** tab, select one or more plugins to clean.
* With the plugin selected, right-click and click **Clean with tes3cmd**.
* After the process is over, close the window.

{% hint style="warning" %}
Clean all mods except for the following:

* **the vanilla .esm files**
* **Beautiful Cities of Morrowind**
* **Fixes for Purists**

{% endhint %}

## 04 Synchronizing mod masters

* Run Wrye Mash (**mash64**) in Mod Organizer 2.
* In the **Mods** tab, you will see a list with all your plugins, both active and inactive. Plugins that do not need to have their masters synchronized have a green box next to them. Those that do need to have their masters synchronized will have a box of a different color.
* Click on the faulty plugin, and a panel to the right will display the plugin's masters. Right click on either of them, and an **Update Masters** window will appear. Click **Yes**.
* Once the window has closed, click on the **Save** button further below the same panel.
* Repeat this process for each of the faulty plugins.

## 05 TES3Merge

{% hint style="info" %}
For record conflicts, we use **TES3Merge**, generating a **Merged Objects.esp** file which we will also place at the end of our load order.
{% endhint %}

* Run TES3Merge in Mod Organizer 2.
* The tool will generate a Merged Objects.esp, solving conflicts in your load order.
* Activate **Merged Objects.esp** at the end of your load order.

## 06 Updating and repairing saves

* Run Wrye Mash (**mash64**) in Mod Organizer 2.
* In the **Saves** tab, you will see a list with all your saves. Saves that do not need to be synchronized have a **purple box** next to them. Those that do need to have their masters synchronized will have a box of a different color.
* Click on the faulty save, and a panel to the right will display the save's masters and plugins. Right click on any of them, and an **Update Masters** window will appear. Click **Yes**.
* Should you have uninstalled plugins in an on-going save, an **Update Masters** window will appear telling you some masters were automatically deselected (as they are no longer present in your load order). Read the description on the box, as it tells you how to proceed if this isn't what you expected to happen. Otherwise, click **OK**.
* Once the window has closed, right click on the **Master** header above your save's masters and plugins, and click **Sync to Load List**.
* Click on the **Save** button further below the same panel.

The next step is to repair our updated save.

* Right click on the save updated in the previous step, and click on **Repair All**. Wrye Mash will repair your save file.
* You will get a message window with two possible outcomes: your save has been repaired by Wrye Mash, or Wrye Mash will tell you no problems where found. Close the window.

{% hint style="warning" %}
If reair all fails, you need to repair two esps:

* Run Wrye Mash (**mash64**) in Mod Organizer 2.
* In the **Mods** tab, select `BM_S_Inn - (Vanilla Inns - Animated Morrowind).ESP`
* Right click -> **Repair Refs**
* In the **Mods** tab, select `Know Thy Ancestors - TR.ESP`
* Right click -> **Repair Refs**

{% hint style="endhint" %}

## 📃 07 MGXE

{% hint style="info" %}
Recreate Distant Land
{% endhint %}

* Run **MGE XE** in Mod Organizer 2.
* In the **Distant Land** tab, click **Distant land generator wizard**.
* Click **Select all**. This will select all plugins for distant land generation, both active and unactive.
* Click **Continue**.
* Click **Run above steps using saved / default settings**.
* Click **Finish** when the process is over.

## 08 Run the game

* ✨If you're on OpenMW, export your mods with Menu > Tools > Tool Plugins > `Export to OpenMW`
* Run the game through MO2

### 📃 Mod Config Menu

In the **Mod Config Menu**, I recommend these options:

Required (or strongly recommended)

* **Improved Vanilla Levelling:** DISABLE Retroactive Health Calculation
* **Weather Adjuster:** Disable sky texture changes -> On

Personal Preference

* **Security Enhanced:** Pick up by default -> Off
* **Map and Compass:** Optionally select map
* **Realistic Repair:** Loot condition -> 25% - 75%
* **Abot's smart journal:** Everything on, except
  * Add a prefix ... -> No Prefix
  * [ ] Add quest identifier -> Off
  * [ ] Add source mod name -> Off
  * [ ] Add source mod Author -> Off
  * [ ] Open first URL -> Off
  * [ ] Adjust bookmark size -> Off
* **Sophisticated Save System:**
  * Number of auto-saves -> 10
  * Minimum time between -> 5
  * Autosave timer duration -> 20

### Settings

**Character Sound Overhaul:** The author recommends you set the Footsteps volume to minimum in your in-game audio settings.
