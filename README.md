# mario64hacks
Collection of hacks and modifications I've done for Super Mario 64

## Mario64LevelSelectPatch.ppf

A patch to enable the debug level select function that remains embedded in the final Super Mario 64 code.

Seemingly the only change is in a single byte:
``` 
0x00269F8F: 0C -> 38 
```

Apply the patch to a clean, extended NTSC version Super Mario 64 rom. Upon applying the patch, the save file select screen will be replaced with the level select screen.

From The Cutting Floor wiki on Mario 64 debug content:
> *When a level is selected, Mario will automatically be sent to the first Star, bypassing the Star selection screen. Exiting a course via Star collection, death, or the pause menu will bring you back to the level select screen. Attempting to access one of the removed entries causes the game to reset.*

Patch was made with:
```
Super Mario 64 (U) [!].z64
Size: 8,338,608
CRC32: 3CE60709
```
