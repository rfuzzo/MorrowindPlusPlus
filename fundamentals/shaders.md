# SHADERS AND PATCHES

## Patches

⭐ [**Beautiful Cities of Morrowind - Patches**](https://www.nexusmods.com/morrowind/mods/49231)\
Patches for various mods

* Files to install:
  * **Beautiful Cities of Morrowind - Patches**

* On MO2 installation, check the following options in the installer:
  * [x] 📃 Ashfall interop
  * [x] Ashlander Traders Remastered
  * [x] Bounty Hunter Assignments
  * [x] Concept Art Plantations
  
  * [x] Ebonheart Underworks
  * [x] Far From Home
  * [x] Foreign Quarter Market Square
  * [x] Glass Domes

  * [x] Logs on Fire
  * [x] Main Quest Overhaul
  * [x] Mamaea Awakened
  * [x] Mandas Manor

  * [x] OAAB Foyada Mamaea Overhaul
  * [x] OAAB Pomegranates
  * [x] Patch for Purists
  * [x] Province Cyrodiil
  * [x] 📃 Realistic Repair Addon
  * [x] Rise of House Telvanni 2.0

  * [x] Store Entrance Chimes
  * [x] Strider Port Lights
  * [x] Tamriel Rebuilt
  * [x] Tel Aruhn Chronicles quest and Yansirramus Overhaul addon
  * [x] The Publicans

  * [x] Velothi Wall Art
  * [x] Velothi Wall Art Re-Addon

{% hint style="warning" %}
Do not use the Publicans patch, it is outdated
{% hint style="endhint" %}

[**Various compatibility patches for HOTV Tomb of the Snow prince Solstheim Overhaul**](https://www.nexusmods.com/morrowind/mods/48422)\
 Various patches, including the White Wolf of Lokken, Wanderes of Solstheim, Children of Morrowind, Thirsk Expanded more....an ongoing project

* Files to install:
  * **Various Patches for Tomb of the Snow prince - All in One**

* Double click the mod in MO2 and go to the **Optional ESPs** tab, move to the left (make optional):
  * [x] `BT_Whitewolf_2_0_TOTSP.esm`
  * [x] `Grandfather Frost - TOTSP.ESP`
  * [x] `Thirsk Expanded for TOTSP.ESP`
  * [x] `Tomb of snow prince_MW_Chilren_Patch.ESP`

{% hint style="warning" %}
After installation

* Run Wrye Mash (**mash64**) in Mod Organizer 2.
* In the **Mods** tab, select `BM_S_Inn - (Vanilla Inns - Animated Morrowind).ESP`
* Right click -> **Repair Refs**

{% hint style="endhint" %}

[**Morag Tong Polished - BCoM Patch**](https://www.nexusmods.com/morrowind/mods/51194)\
One of the NPCs added by "MTP" ends up being suspended in the empty void if you use it alongside with the "Beautiful Cities of Morrowind". This patch returns him to the intended position. Also works fine with a replacer plugin provided by "Vanilla friendly wearables expansion".

* Files to install:
  * **After the Blight (BCoM)**
  * **Morag Tong Polished - BCoM Patch**

⭐ [**alvazir's various patches**](https://www.nexusmods.com/morrowind/mods/48955)\
Collection of compatibility patches, fixes, mod expansions and tiny mods.

* Files to download:

  * **Miscellaneous Patches**

    * On MO2 installation, check the following options in the installer:
      * [x] 01 Misc
      * [x] 02 Script Fix
      * [x] 03 Creature Leveled Lists

    * Available esps:
      * AliceL93 Vanilla Quest Tweaks - Script Fix.esp
      * AliceL93 Vanilla Quest Tweaks - TR_Factions Compatibility Patch.esp
      * Ebonheart_Underworks - Disable Rebirth Question.esp
      * Library of Vivec Overhaul - Full - Dialogue Fix.esp
      * Morrowind - Tombs Leveled Lists Flag Fixed.esp
      * OAAB Brother Junipers Twin Lamps - Camonna Tong Compatibility Patch.esp
      * OAAB Brother Junipers Twin Lamps - Script Fix.esp
      * Solstheim Tomb of The Snow Prince - Bloodmoon Rebalance.esp
      * Tribunal - Rare Durzogs In Vvardenfell Caves.esp
      * Wares-base - Adamantium Armor - Rare.esp

⭐ [**Null's Minor Patches**](https://www.nexusmods.com/morrowind/mods/55897)\
Most patches are to prevent errors in the MWSE.log file, and do not substantially change the behavior of the mod.

* Patch for Beautiful Cities of Morrowind v3.2.3
* Patch for Character Sound Overhaul v1.1
* Patch for Graphic Herbalism v1.04
* Patch for Heat Haze v1.1
* Patch for Muse
* Patch for Spells Reforged v1.1
* Patch for Tamriel_Data v11.0

## Shaders

⭐📃 [**Pixel Shader Style Water for MGE XE**](https://www.nexusmods.com/morrowind/mods/50044)\
A modernized version of the pixel shader water from vanilla Morrowind, which aims to replicate the texture, transparency, and artistic feeling of the original mercurial water, without duplicating its low resolution.

⭐✨ [**Zesterer's OpenMW Shaders**](https://github.com/zesterer/openmw-shaders/tree/openmw-0.48)\
Photorealistic shaders for Morrowind

{% hint style="info" %}
Per-pixel lighting enabled
Light clamping disabled
{% endhint %}

⭐✨ [**Zesterer's Volumetric Cloud & Mist Mod for OpenMW**](https://github.com/zesterer/openmw-volumetric-clouds)\
 A volumetric clouds mod for OpenMW

{% hint style="info" %}
Enable post-processing shaders in your settings.cfg.
{% endhint %}

## Shader setup

* Run MGE XE in Mod Organizer 2.
* In the **Graphics tab**, click **Enable shaders**.
* Click **Shader setup...**.
* On the **Set active shaders** window, click **Modding >>>**.
* Double click on the corresponding shader under **Available shaders** to activate.
* Under **Active Shaders** have the following:

```text
SSAO HQ
Underwater Interior Effects
Invisibility
EdgeAA
deband_fogawarev3
Underwater Effects
Sunshafts
Special Process
Eye Adaptation (HDR)
heathaze
r0_qk_shaker
skoomaesthesia
warp
```

* Click **Save** after setting up your shader chain.

{% hint style="info" %}
Note that all of these shaders, minus the ones added by mods and which thus won't work without them enabled, are optional. In particular, **Special Process** tends to be divisive.
{% endhint %}
