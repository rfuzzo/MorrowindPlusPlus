# SHADERS AND PATCHES

## Patches

⭐ [**Even Seedier Eight Plates - Morag Tong Polished Patch**](https://www.nexusmods.com/morrowind/mods/49236)\
 VIsual overhaul of the Eight Plates tavern in Balmora, combined with an expansion of the NPC and dialogue overhaul from Von Djangos' The Seedy Plates

* Files to install:
  * **ESEP - Morag Tong Polished Patch**

{% hint style="warning" %}
You need to rename the .esp file in this mod! In MO2, double click the mod and go to the Filetree tab. Right click an rename the esp to `Morag Tong Polished.esp`
{% endhint %}

![Screenshot](../pictures/ESEP_rename.jpg)

{% hint style="info" %}
Even Seedier Eight Plates is merged into BCOM - no need to install the main file
{% endhint %}

⭐ [**Beautiful Cities of Morrowind - Patches**](https://www.nexusmods.com/morrowind/mods/49231)\
Patches for various mods

* Files to install:
  * **Beautiful Cities of Morrowind - Patches**

{% hint style="info" %}
On MO2 installation, it does not matter if you install too many mods, we will go over the individual ESPs later again:
{% endhint %}

* On MO2 installation, check the following options in the installer:
  * Patches
    * [x] Patch for Purists
    * [x] Concept Art Plantations
    * [x] Arvesa - An Armigers Tale
    * [x] Mandas Manor
    * [x] Siege at Firemoth
  * OAAB Foyada Mamaea Overhaul -> **OAAB Foyada Mamaea Overhaul**
  * Animated Morrowind -> **Animated Morrowind**
  * Rise of House Telvanni -> **RoHT 2.0**

  * Abots Boats -> **Abots Boats**
  * Abots Boats for Tomb of the Snow Prince -> **Boats for TOTSP**
  * [x] Abot's Gondoliers -> yes
  * Abots Silt Striders -> **Abots Silt Striders**
  * TR_Travels -> **TR_Travels**
  * Yet Another Guard Diversity -> **Regular**
  * More Patches
    * [x] Province Cyrodiil
    * [x] Ebonheart Underworks

  * Select all that apply
    * [x] Morrowind Anticheese
    * [x] Bounty Hunter Assignments
    * [x] Realistic Repair Addon
  * Mines and Caverns -> **Mines and Caverns**

  * Select all that apply
    * [x] Velothi Wall Art
    * [x] Velothi Wall Art Re-Addon
    * [x] Area of effect Arrows

  * Select all that apply
    * [x] The Publicans
    * [x] Glass Domes
    * [x] Store Entrance Chimes
    * [x] Far From Home

  * Select all that apply
    * [x] 📃 The Sanguine Rose
    * [x] Main Quest Overhaul
    * [x] Mamaea Awakened
    * [x] 📃 Ashfall interop
    * [x] OAAB Pomegranates
    * [x] Tel Aruhn Chronicles quest and Yansirramus Overhaul addon
    * [x] Foreign Quarter Market Square

[**Various compatibility patches for HOTV Tomb of the Snow prince Solstheim Overhaul**](https://www.nexusmods.com/morrowind/mods/48422)\
 Various patches, including the White Wolf of Lokken, Wanderes of Solstheim, Children of Morrowind, Thirsk Expanded more....an ongoing project

* Files to install:
  * **The Moldy Horker - TOTSP Solstheim - Animated Morrowind**
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

⭐ [**Ashlander Traders - Remastered - BCOM and Wares**](https://www.nexusmods.com/morrowind/mods/48009)
Brother Juniper's excellent Ashlander Traders mod, edited for compatibility and extra dialogue. Adds Ashlander Traders who will sometimes appear in Balmora, Ald-ruhn, or Suran.

* Files to install:
  * **Ashlander Traders Remastered - BCOM and Wares**

⭐ [**Ownership Overhaul Patches**](https://www.nexusmods.com/morrowind/mods/49232)\
Compatibility patches for canton mods.

* On MO2 installation, check the following options in the installer:
  * [X] 00 Glass Domes of Vivec
  * [ ] 01 No-Frills Closed Molag Mar
  * [ ] 01 No-Frills Open Arena
  * [x] 02 Solstheim Tomb of the Snow Prince

## Shaders

⭐📃 [**Pixel Shader Style Water for MGE XE**](https://www.nexusmods.com/morrowind/mods/50044)\
A modernized version of the pixel shader water from vanilla Morrowind, which aims to replicate the texture, transparency, and artistic feeling of the original mercurial water, without duplicating its low resolution.

⭐📃 [**MGE XE Shader Pack**](https://github.com/Sigourn/nerevarrising/blob/master/mods/MGE%20XE%20Shader%20Pack.7z)\
A compilation of a handful of community-made shaders.

{% hint style="info" %}
[**External Link**](https://github.com/Sigourn/nerevarrising/raw/master/mods/MGE%20XE%20Shader%20Pack.7z) to the download.
{% endhint %}

* On MO2 installation, check the following options in the installer:
  * [x] 00 Core

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
