# Finishing

{% hint style="info" %}
If you just installed this modlist or ar updating it you need to always run the following steps in this order:
{% endhint %}

## 01 Updates

* Run **MWSE-Update** in Mod Organizer 2.
* Run **Mlox-Update** in Mod Organizer 2.

## 02 MLOX

* Run **MLOX** in Mod Organizer 2.
* Wait for it to load
* Check the **Status** and **Messages** Tabs for errors or incompatibilities
* Click **Update Load Order**
* Close the Window.

## 03 Wrye Mash

{% hint style="info" %}
**This section is based on:** Sigourn @ [https://github.com/Sigourn/nerevarrising/blob/master/main.md](https://github.com/Sigourn/nerevarrising/blob/master/main.md)
{% endhint %}

### Synchronizing mod masters

* Run Wrye Mash (**mash64**) in Mod Organizer 2.
* In the **Mods** tab, you will see a list with all your plugins, both active and inactive. Plugins that do not need to have their masters synchronized have a green box next to them. Those that do need to have their masters synchronized will have a box of a different color.
* Click on the faulty plugin, and a panel to the right will display the plugin's masters. Right click on either of them, and an **Update Masters** window will appear. Click **Yes**.
* Once the window has closed, click on the **Save** button further below the same panel.
* Repeat this process for each of the faulty plugins.

### Conflict resolution

{% hint style="info" %}
For leveled list conflicts, we use **tes3cmd**, generating a **multipatch.esp** file which we will place at the end of our load order.
{% endhint %}

* In the **Mods** tab, click the **Misc** header and go to **TES3cmd** -> **Create MultiPatch**. Click **Yes** on the prompt.
* tes3cmd will now generate the multipatch. After the process is over, click **OK**.
* **multipatch.esp** will now be present at the end of your load order.

### Updating and repairing saves

* In the **Saves** tab, you will see a list with all your saves. Saves that do not need to be synchronized have a **purple box** next to them. Those that do need to have their masters synchronized will have a box of a different color.
* Click on the faulty save, and a panel to the right will display the save's masters and plugins. Right click on any of them, and an **Update Masters** window will appear. Click **Yes**.
* Should you have uninstalled plugins in an on-going save, an **Update Masters** window will appear telling you some masters were automatically deselected (as they are no longer present in your load order). Read the description on the box, as it tells you how to proceed if this isn't what you expected to happen. Otherwise, click **OK**.
* Once the window has closed, right click on the **Master** header above your save's masters and plugins, and click **Sync to Load List**.
* Click on the **Save** button further below the same panel.

The next step is to repair our updated save.

* Right click on the save updated in the previous step, and click on **Repair All**. Wrye Mash will repair your save file.
* You will get a message window with two possible outcomes: your save has been repaired by Wrye Mash, or Wrye Mash will tell you no problems where found. Close the window.

## 04 TES3Merge

{% hint style="info" %}
For record conflicts, we use **TES3Merge**, generating a **Merged Objects.esp** file which we will also place at the end of our load order.
{% endhint %}

* Run TES3Merge in Mod Organizer 2.
* The tool will generate a Merged Objects.esp, solving conflicts in your load order.
* Activate **Merged Objects.esp** at the end of your load order.

## 05 MLOX silent mode

{% hint style="info" %}
After creating the **multipatch.esp** and the **Merged Objects.esp**, these need to be in the correct order. The fastest is to simply run MLOX again
{% endhint %}

* Run **MLOX silent mode** in Mod Organizer 2.

## 06 MGXE

{% hint style="info" %}
Recreate Distant Land
{% endhint %}

* Run **MGE XE** in Mod Organizer 2.
* In the **Distant Land** tab, click **Distant land generator wizard**.
* Click **Select all**. This will select all plugins for distant land generation, both active and unactive.
* Click **Continue**.
* Click **Run above steps using saved / default settings**.
* Click **Finish** when the process is over.

## Run the game

* Run the game through MO2
