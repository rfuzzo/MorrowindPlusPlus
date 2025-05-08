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

[**Class Starting Spells for ME v3**](https://www.nexusmods.com/morrowind/mods/47111)\
Patch for Class Starting Spells to work with ME 3.0.0+

[**OAAB to RR Telvanni Consistency**](https://www.nexusmods.com/morrowind/mods/56187)\
Changes the RR Telvanni Lighthouse crystals to OAAB blue, or changes the OAAB telvanni crystals to RR white.

[**Katya's Patches and mod recommendations**](https://www.nexusmods.com/morrowind/mods/56060)\
Here are some patches I made for my modlist, maybe it'll be useful to someone.

* Files to download:

  * **Ald Gash Lighthouse Patch for Rocky West Gash**
  * **Snowy Holly Bushes Patch**

[**momw-patches**](https://modding-openmw.gitlab.io/momw-patches/)\
Patches made by the Modding-OpenMW.com community.

* On MO2 installation, check the following options in the installer:
  * [x] 05 AFFresh + Samarys Ancestral Tomb Expanded Patch
  * [x] 10 Ebonheart Underworks MOMW Patch
  * [x] 11 Mamaea Awakened OpenMW Patch
  * [x] 21 Imperial Factions Patched
  * [x] 24 BCOM + Dagon Fel Lighthouse + Remiros’ Groundcover patch
  * [x] 56 Quest Voice Greetings + Tamriel Data Patch
  * [x] 58 OAAB Shipwrecks+Justice for Khartag MOMW Patch

[**Mono's Minor Moddities**](https://www.nexusmods.com/morrowind/mods/53027)\
Various minor mods patched together mostly as small improvements or patches to other popular mods.

* Files to download:

  * **Tomb of the Snow Prince - PA and GitD Patch**

[**Various tweaks and fixes**](https://www.nexusmods.com/morrowind/mods/43795?tab=files)\
Small mods, tweaks and fixes.

* Files to download:

  * **familiar_faces_fixes**

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
