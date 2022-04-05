# Fixes

## Bug fixes

[**Patch for Purists**](https://www.nexusmods.com/morrowind/mods/45096)\
Unofficial patch for The Elder Scrolls III: Morrowind Game of the Year Edition that aims to make the game completely bug-free (within the abilities of Construction Set). It diverges from later versions of the community patches in that it takes a more conservative approach about what it considers a bug.

[**Unofficial Morrowind Official Plugins Patched**](https://www.nexusmods.com/morrowind/mods/43931?)\
Fixes many issues present in Bethesda's original Official Plugins.

Files to install:

* **UMOPP 3.1.0** (Main files)
* After installation, hide all of the mod's plugins minus **bcsounds.esp** and **master\_index.esp**.

[**Area Effect Arrows Integrated**](https://www.nexusmods.com/morrowind/mods/47745)\
Alternative version of the official plugin adding new arrows that explode on impact. Tweaked to distribute arrows across leveled lists and vendors instead of dumping them all in one shop.

* After installation, hide all of the mod's plugins minus **Area Effect Arrows Integrated.ESP**.

[**Better Propylon Teleport Script**](https://www.nexusmods.com/morrowind/mods/46364)\
The Warp Script for the Propylon Indices will now prompt you before teleporting.

* After installation, hide all of the mod's plugins minus **Better Propylon Teleport Warp-Master Index.ESP**.

[**Adamantium Ore Fix ESP Replacer**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Adamantium%20Ore%20Fix%20ESP%20Replacer.7z)\
Allows the player to find the exact amount of Adamantium Ore needed to craft Bols Indalen's custom Adamantium Armor. Includes fixes from Patch for Purists.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/47068) to original mod by **Half11**.

[**Divayth Fyr Puzzle Fixed**](https://www.nexusmods.com/morrowind/mods/45155)\
Reworks Divayth Fyr’s puzzle so that you require the correct key to open the chests as well as locking up all the artifacts, which now require the final key to be opened.

* On MO2 installation, check the following options in the FOMOD installer:
  * [x] Patch for Purists
  * [x] Ownership Overhaul

[**Dubdilla Location Fix**](https://www.nexusmods.com/morrowind/mods/46720)\
Moves the entrance to the cavern of Dubdilla to a more logical place according to in-game information.

[**Services Restored**](https://www.nexusmods.com/morrowind/mods/47068)\
Adds the missing master trainer for Medium Armor, Cinia Urtius.

[**Silt Strider Animation Restored**](https://www.nexusmods.com/morrowind/mods/44150)\
Restores previously unused Silt Strider animation - it was present in the model, but never played in the game itself because of the lack of the necessary script. It also comes with a previously unused sound.

[**Under Construction**](https://www.nexusmods.com/morrowind/mods/50285)\
Construction materials and scaffolding are now visible at the Great House strongholds during construction of the later stages.

## Mesh fixes

⭐ [**Correct UV Rocks**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Correct%20UV%20Rocks.7z)\
Fixes UV mapping on rocks and stones.

> ℹ️ [**Link**](https://mw.modhistory.com/download-56-12003) to original mod by **Nich**. The featured version omits a faulty mesh.

⭐ [**Fix Those Bastard Rope Fences**](https://www.nexusmods.com/morrowind/mods/45741)\
Modifies collision boxes on rope-related meshes, player and NPC's hitboxes to prevent getting stuck.

⭐ [**Morrowind Optimization Patch**](https://www.nexusmods.com/morrowind/mods/45384)\
Greatly improves performance and fixes some mesh errors.

* On MO2 installation, check the following options in the BAIN installer:
  * [x] 00 Core
  * [x] 01 Lake Fjalding Anti-Suck\
    Increases performance around Lake Fjalding by replacing several of the smaller meshes with larger, merged ones. Has no impact on visuals.
  * [x] 02 Weapon Sheathing Patch\
    Compatibility patch for Weapon Sheathing. Makes weapon sheaths show the fixed MOP weapon meshes instead of the vanilla ones.
  * [x] 03 Chuzei Fix\
    Fixes neck problems with the Native Chuzei Bonemold Helm.
  * [x] 04 Better Vanilla Textures\
    Includes several vanilla textures with fixed alphas and several other changes made specifically for MOP. Also fixes a lot of broken textures and makes textures that were supposed to be seamless actually seamless.

> ℹ️ We will install **Weapon Sheathing** in the **Visuals** section, and load it before this mod for **MOP** to patch it as intended.

⭐ [**Project Atlas**](https://www.nexusmods.com/morrowind/mods/45399?)\
Optimizes the most performance heavy areas of vanilla Morrowind through texture atlases.

Files to install:

* **Project Atlas** (Main files)
* On MO2 installation, check the following options in the BAIN installer:
  * [x] 00 BATs
  * [x] 00 Core
  * [x] 01 Textures - Vanilla
  * [x] 06 Glow in the Dahrk Patch\
    Compatibility patch for Glow in the Dahrk. Uses compatible meshes.
  * [x] 07 Graphic Herbalism Patch\
    Compatibility patch for Graphic Herbalism. Uses compatible meshes.

> ℹ️ We will install **Graphic Herbalism** and **Glow in the Dahrk** in upcoming sections, and load them before Project Atlas for it to patch them as intended.

> ⚠️ Note that **Project Atlas** utilizes its own texture sets for its edited meshes, meaning any retexture designed with the vanilla meshes in mind will require a patch for it to work alongside this mod.

⭐ [**Creature VFX Restoration**](https://www.nexusmods.com/morrowind/mods/46194)\
Restores visual effects on creatures that weren't displayed for technical reasons.

⭐ [**Improved Thrown Weapon Projectiles**](https://www.nexusmods.com/morrowind/mods/44763)\
Mesh replacer for thrown weapon projectiles that makes them fly pointy end forward and, in some cases, spin in the air.

* On MO2 installation, right-click on **Data Files**.
* Click **Set as data files directory** and click **OK**.

[**Better Scamps**](https://www.nexusmods.com/morrowind/mods/48008)\
Fixes the Scamp mesh, reducing distortion, seams, and other UV errors.

* After installation, hide the mod's **Textures** folder.

> ℹ️ This omits the Scamp's retexture, since **Intelligent Textures** uses a vanilla-friendly high resolution texture.

[**Correct UV Mudcrabs**](https://www.nexusmods.com/morrowind/mods/42130)\
Fixes the Mudcrab mesh, reducing distortion and other UV errors.

* On MO2 installation, expand the **Correct Mudcrab** and **Regular** folders.
* Right-click on **Data Files**.
* Click **Set as data files directory** and click **OK**.

[**Glowing Flames**](https://www.nexusmods.com/morrowind/mods/46124)\
Flames are now glow mapped and/or properly illuminated.

* After installation, hide the mod's **Glowing Flames - TrueLightsAndDarkness Tweaks.ESP** plugin.

## MWSE bug fixes

⭐ [**Expeditious Exit**](https://www.nexusmods.com/morrowind/mods/45634)\
Forces the game to instantly close on exit.

[**Consistent Enchanting**](https://www.nexusmods.com/morrowind/mods/50029)\
Carries over unique item information, such as condition and script data when enchanting items.

[**Fortify MAX**](https://www.nexusmods.com/morrowind/mods/49825)\
Causes Fortify Magicka and Fortify Fatigue to affect the maximum as well as the current stat.

[**Immersive Run Fix**](https://www.nexusmods.com/morrowind/mods/45947)\
Normalizes the player's movement speed, ensuring they run at a consistent speed even during diagonal movement.

[**Just Drop It**](https://www.nexusmods.com/morrowind/mods/49557)\
Dropped items and corpses are automatically positioned and oriented to align with the ground.

[**Loading Doors Lock Tune**](https://www.nexusmods.com/morrowind/mods/46094)\
Automatically synchronizes linked doors locked/unlocked state on activate, lock/unlock by spell, unlock by lockpick, key. Makes loading doors play close sound a short time after opening.

[**Putting Power In Willpower (Necro Edit)**](https://github.com/Sigourn/morrowind-sharprepository/blob/main/Putting%20Power%20in%20Willpower%20\(Necro%20Edit\).7z)\
Rebalances the willpower-based spell resist mechanic, giving all in-game actors, Player, NPCs and Creatures an ability to shrug off spells through the sheer force of will, as it is implied by the attribute's description.

> ℹ️ [**Link**](https://www.nexusmods.com/morrowind/mods/45742) to original mod by **R-Zero**. The featured version includes fixes by **Necrolesian**.

[**Quest Skill Reward Fix**](https://www.nexusmods.com/morrowind/mods/48269)\
Makes the game treat skill increases from quests as if there were raised via normal means, solving numerous problems with how the game treats these skill increases.

[**Skill Increase GMST Fix**](https://www.nexusmods.com/morrowind/mods/48029)\
Fixes several engines related to GMSTs used when raising skills via NPC training and skill books.

[**Thrown Projectiles Revamped**](https://www.nexusmods.com/morrowind/mods/49609)\
Corrects thrown projectiles inflicting twice their listed damage, by halving their damage output.
