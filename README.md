# Wetrix (1998, N64)
It's everyone's favorite water game, and now you can look at why it makes the system chug (because water)

## Instructions:
Add your legally obtained US Wetrix to the base of this repository, rename it to `baserom.z64` and run `splat`.
European and Japanese versions currently not being looked into.

## Curiosities
* Game is in six languages. All related strings are uncompressed.
* F3DEX.NoN (1.21) microcode
* Compiler: GCC 2.7.2 (SN) (Build 0001) (thx queueRAM, confirmed by galaxyhaxz)
* Does not seem to use overlays..?
* A few shared assets with PC version

## Regarding the PC Version
* MSVC 4.1, uses DirectDraw and plays music from CD through WinMM.
* Board is software rasterized at a fixed perspective
* Very little of the assets are binary data things. A ton of bitmaps, text files (for each language) and audio files.
* GOG release uses a DLL replacement for WinMM so it instead plays .ogg conversions of the soundtrack.

I initially wanted to do the PC version first but MSVC 4.x being a victim of compiler entropy brings more misery than
I can endure, plus tooling for splitting exes is all over the place. Aren't old compilers awesome?
