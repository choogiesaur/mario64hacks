# mario64hacks
Collection of hacks and modifications I've done for Super Mario 64

## Mario64LevelSelectPatch.ppf

A patch to enable the debug level select function that remains embedded in the final Super Mario 64 code.

Seemingly the only change is in a single byte:
> 0x00269F8F: 0C -> 38

Apply the patch to a clean, extended NTSC version Super Mario 64 rom. Patch was made with:
> Super Mario 64 (U) [!].z64
> Size: 8,338,608
> CRC32: 3CE60709
