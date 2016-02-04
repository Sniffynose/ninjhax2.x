ninjhax 2.x - Clean Boot
========================

-Removes all colors except for fail state (BSOD lol)
-Removes all debug text
-Adds comments for each colour step to locate easier *note color hex codes are read right to left*

*** This mod works best with a custom image setup using menuhax_manager, it will remove the intial garbage on screen and improve boot rates. (Image can just be black even) ***

To use: From the main folder: python scripts/buildVersion.py "N9.2.0-20U" for example will only make the ropbin payload for New 3ds on version 9.2.0.20U, adding the --enableotherapp line right after the above string will build the otherapp_ropbin_payload type. Outputs go into the P/R/Q folders R= ropbin 65kb, Q= QRCODE, P= Otherapp_ropbin 41kb


To compile you need global var CTRULIB to link to the included libctru folder (must "make" this first)

You will also need blowfish_processed.bin and blz.exe in your scripts directory, google is your friend.

zlib1.dll, libz.a and armips.exe will also be needed inside various devkit paths (follow the errors for hints).

DevkitPro ARM 3ds/python and proper system path links etc.

Hopefully this will help solve the common compile errors. Make sure to use the lastest builds, older ones will fail. Only the libctru and libctru-fpic included should be used as they are custom older builds.

### Credits ###

- All original ROP and code on this repo written by smea
- yellows8, plutoo
