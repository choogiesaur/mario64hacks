# mario64hacks
Collection of hacks and modifications I've done for Super Mario 64

## Mario64LevelSelectPatch.ppf

A patch to enable the debug level-select function that remains embedded in the final Super Mario 64 binary.

Seemingly the only change is in a single byte:
``` 
0x00269F8F: 0C -> 38 
```

## Mario64EnhancedLevelSelectPatch.ppf

My enhanced original patch that both enables the debug level select screen in Super Mario 64 and changes the stage titles. The default titles either reference the Japanese names or have graphical glitches. This for the most part fixes that.

Apply either patch to a clean, extended NTSC version Super Mario 64 rom. Use [sm64extend found here](https://sm64hacks.com/hacktools.php "SM64 Hack Tools") to expand the rom to 64MB first.
Upon applying the patch, the save file select screen will be replaced with the level select screen. Patch was made with the following file, processed with sm64extend:
```
Super Mario 64 (U) [!].z64
Size: 8,338,608
CRC32: 3CE60709
```

**Notes from The Cutting Floor wiki on Mario 64 debug content:**
> *When a level is selected, Mario will automatically be sent to the first Star, bypassing the Star selection screen. Exiting a course via Star collection, death, or the pause menu will bring you back to the level select screen. Attempting to access one of the removed entries causes the game to reset.*
