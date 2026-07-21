# Wetrix (1998, N64)
It's everyone's favorite water game, and now you can look at why it makes the system chug (because water)

## how 2
put US Wetrix as the baserom in the folder and do `splat` magic. 
zero plans for the PAL or JP versions, I can barely even comprehend *one* wetrix

# In Serious Need of Help
I have no idea what I'm doing and solely know how to write C for 5+ years and occasional linux daily driving.
Contact me at unevenprankster on discord or open an issue/pr if unlike me you actually know what you're doing.

## Curiosities
* Game is in six languages. All related strings are uncompressed.
* F3DEX.NoN (1.21) microcode
* Suspected compilers: GCC 2.7.2 KMC or 2.7.2 (SN) (Build 0001) (thx queueRAM!)
* Current split is grossly wrong since `main` is nowhere to be found except in the assets binary blob.
* Does not seem to use overlays
* A few shared assets with PC version

## Regarding the PC Version
* MSVC 4.1, uses DirectDraw and plays music from CD through WinMM.
* Board is software rasterized at a fixed perspective
* Very little of the assets are binary data things. A ton of bitmaps, text files (for each language) and audio files.
* GOG release uses a DLL replacement for WinMM so it instead plays .ogg conversions of the soundtrack.

I initially wanted to do the PC version first but MSVC 4.x being a victim of compiler entropy brings more misery than
I can endure, plus tooling for splitting exes is all over the place. Aren't old compilers awesome?