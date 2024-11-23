# Changelog

## Version 4.0.0 - 23.11.2024
* Added [Syllabore](https://github.com/kesac/Syllabore) support for Name Generation
* Made the Names more variable and not fully stuck to what their EditorID would be.
* Renamed more parts of the Patcher to Synthesis RPG Loot from Halgaris RPG Loot.
* Reduced the amount of logging and added a toggle to disable logging for individual items for better performance:
  * Runtime with logging for individual items disabled 1.8 min.
  * Runtime with logging for individual items enabled 2 min.

(Times recorded using the default settings and all the Anniversary Edition DLC Content Installed on an AMD Ryzen 5 7600X CPU)

## Version 3.2.0 - 06.04.2024
* Fixed unplayable armor and weapon records being used in the patcher

## Version 3.1.1 - 04.04.2024
* Updated Synthesis dependency

## Version 3.1.0 - 03.04.2024
* Removed only process constructable items because it isn't creating the limit that it is intended for.
* Fixes for SkyrimVR and the Plugin Header Version 1.71

## Version 3.0.0 - 01.04.2024
* Complete rewrite of the item distribution method
  * Added filters with sane default values to filter out "dummy" enchantments that are just used for VFX
  * Allows for more flexibility and control than any previous version
    * please check the [README.md](README.md) for more details
  * Should be less prone to breaking even on bigger setups
    * I still advise caution since the file size of the resulting ESP could turn out bigger than 
      the `Skyrim.esm` (The default settings of this patcher with a fresh steam install results 
      in an ESP that is over double the size than the largest official DLC) and I can't guarantee how
      or if the Engine and tools like xEdit can handle that when it gets bigger!!
* Item and Enchantment Names now list all enchantments
  * added a config option to configure the separators for this
* lowered the total output size of the patch
*increased patching performance
