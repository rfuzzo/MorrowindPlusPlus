# main

####

###

###

###

###

####

####

####

### MOD CONFIG

⭐ [**MWSE Config**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/MWSE%20Config.7z)\
Includes **Mod Config** tweaks for the following mods, as well as additional edits not available through the in-game menu.

* On MO2 installation, check the following options in the BAIN installer:
  * [x] 00 All in One: recommended option. Includes all configuration options.

<details>

<summary>List of configured mods</summary>

* [ ] 01 Sophisticated Save System\
  Sets a minimum time between autosaves of 5 seconds; increases the autosave timer duration to 20 seconds; disables creation of autosaves before and after combat; enables creating of autosaves after changing cells.
* [ ] 02 Clock Block\
  Sets the clock type to game time.
* [ ] 02 Continue\
  Hides the New Game button while in-game to prevent accidental misclicks, and hides the Credits button in the main menu.
* [ ] 02 Essential Indicators\
  Disables immersion breaking indicators, new sneak indicators, and messages; sets the crosshair to Oblivion-style.
* [ ] 02 Quick Equip\
  Assigns the E key as the key for equipping items.
* [ ] 02 Smart Journal\
  Disables unnecessary immersion breaking options and quest prefixes, removing lag when opening the quests and journal menues.
* [ ] 02 UI Expansion\
  Disables auto-select search bar, disables verbose buttons in favor of icons.
* [ ] 03 GMST Menu\
  Makes NPCs less likely to greet you when walking past them; lowers camera view while sneaking; increases the time it takes for containers to respawn to 7 days (from 3).
* [ ] 03 Security Enhanced\
  Disables automatic probe-equip on trapped object activation.
* [ ] 04 Lucky Strike Configures the mod to reduce maximum damage.
* [ ] 04 Magicka Based Skill Progression\
  Disables logging, and slows down skill experience gain per magicka spent.
* [ ] 04 Ashfall\
  Enables death by hunger and thirst; disables potion hydration; slows down tiredness rate by 20%.
* [ ] 05 Controlled Consumption\
  Sets the consumption module to Vanilla NPC Style (Necro Edit).
* [ ] 06 Let There Be Darkness\
  Sets the cell lighting overrides to use True Lights and Darkness'; comments out a line in the **main.lua** to disable the Lighting Preview feature in order to increase compatibility with **Security Enhanced**.
* [ ] 06 Watch the Skies\
  Sets the chance for vanilla cloud textures to 10%; disables seasonal weather and seasonal daytime hours.
* [ ] 06 Weather Adjuster\
  Makes nights darker; makes fog nicer. [**Comparison slides available here.**](https://imgsli.com/MTUwMjI)
* [ ] 07 AURA\
  Disables player voice taunts.
* [ ] 07 Character Sound overhaul\
  Comments out a line in the **main.lua** to disable MWSE.log spam.

</details>

###

### FINISHING TOUCHES

#### Adjusting mod order and load order

[**Morrowind Sharp MO2 Profile Files**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Morrowind%20Sharp%20MO2%20Profile%20Files.7z)\
Adjusts mod order and load order for Morrowind Sharp to work as intended.

* Extract the files into **C:\Games\Morrowind Sharp\MO2\profiles\Morrowind Sharp**, overwriting when prompted.

#### Synchronizing mod masters

* Run Wrye Mash (**mash64**) in Mod Organizer 2.
* In the **Mods** tab, you will see a list with all your plugins, both active and inactive. Plugins that do not need to have their masters synchronized have a green box next to them. Those that do need to have their masters synchronized will have a box of a different color.
* Click on the faulty plugin, and a panel to the right will display the plugin's masters. Right click on either of them, and an **Update Masters** window will appear. Click **Yes**.
* Once the window has closed, click on the **Save** button further below the same panel.
* Repeat this process for each of the faulty plugins.

#### Cleaning plugins

For general dirty records, we use **Wrye Mash**, automatically cleaning them.

* Run Wrye Mash (**mash64**) in Mod Organizer 2.
* In the **Mods** tab, CTRL+left click on the following plugin:
  * **TheMidnightOil.ESP**
* With the plugin selected, right-click and click **Clean with tes3cmd**.
* After the process is over, close the window.

For specific records we want to delete, we use **TESAME**.

* Run **TESAME** in Mod Organizer 2.
* Delete the following record from **Services Restored.ESP**:
  * NPC **hecerinde**
* Save the plugin as **Services Restored.ESP**, overwriting the original.

> ℹ️ This omits the restoration of Hecerinde's Secret Master tools from [**Services Restored**](https://www.nexusmods.com/morrowind/mods/47068), for consistency with the rest of the Secret Master tools unavailable in the game.

#### Conflict resolution

For leveled list conflicts, we use **tes3cmd**, generating a **multipatch.esp** file which we will place at the end of our load order.

* Run Wrye Mash (**mash64**) in Mod Organizer 2.
* In the **Mods** tab, click the **Misc** header and go to **TES3cmd** -> **Create MultiPatch**. Click **Yes** on the prompt.
* tes3cmd will now generate the multipatch. After the process is over, click **OK**.
* **multipatch.esp** will now be present at the end of your load order.

For record conflicts, we use **TES3Merge**, generating a **Merged Objects.esp** file which we will also place at the end of our load order.

* Run TES3Merge in Mod Organizer 2.
* The tool will generate a Merged Objects.esp, solving conflicts in your load order.
* Activate **Merged Objects.esp** at the end of your load order.

#### Updating and repairing saves

When uninstalling or modifying plugins in an on-going save, Morrowind will greet us with the following message on loading our save:

```
The currently selected master files and plugins do not match the ones used by this save game. 
Errors may occur during load or game play. Do you wish to continue?
```

This means we need to synchronize our save's plugins to our current load order.

* Run Wrye Mash (**mash64**) in Mod Organizer 2.
* In the **Saves** tab, you will see a list with all your saves. Saves that do not need to be synchronized have a **purple box** next to them. Those that do need to have their masters synchronized will have a box of a different color.
* Click on the faulty save, and a panel to the right will display the save's masters and plugins. Right click on any of them, and an **Update Masters** window will appear. Click **Yes**.
* Should you have uninstalled plugins in an on-going save, an **Update Masters** window will appear telling you some masters were automatically deselected (as they are no longer present in your load order). Read the description on the box, as it tells you how to proceed if this isn't what you expected to happen. Otherwise, click **OK**.
* Once the window has closed, right click on the **Master** header above your save's masters and plugins, and click **Sync to Load List**.
* Click on the **Save** button further below the same panel.

The next step is to repair our updated save.

* Right click on the save updated in the previous step, and click on **Repair All**. Wrye Mash will repair your save file.
* You will get a message window with two possible outcomes: your save has been repaired by Wrye Mash, or Wrye Mash will tell you no problems where found. Close the window.

#### Re-running Distant Land

> ℹ️ If this is your first time generating Distant Land, follow the steps found **in this section**. Otherwise, proceed as follows.

* Run MGE XE in Mod Organizer 2.
* In the **Distant Land** tab, click **Distant land generator wizard**.
* Click **Select all**. This will select all plugins for distant land generation, both active and unactive.
* Click **Continue**.
* Click **Run above steps using saved / default settings**.
* Click **Finish** when the process is over.

> ⚠️ For no reason should you ever enable **Remiros' Groundcover** plugins in Mod Organizer 2. These plugins are meant to be used for Distant Land generation only. If you enable them, you will find that you are unable to walk through grass. Likewise, if you generate Distant Land with the plugins enabled, but make the mistake of disabling the entire mod (instead of _just_ the plugins) during gameplay, you will find missing meshes.

#### Updating MWSE

* Run **MWSE-Update.exe** in **C:\Games\Morrowind**.
* A command window will open and close shortly after, having updated MWSE to the latest version.

> ℹ️ Make it a habit to update MWSE whenever you play Morrowind, and particularly when you download recent mods which rely on MWSE. These may have been developed with the latest update in mind.

