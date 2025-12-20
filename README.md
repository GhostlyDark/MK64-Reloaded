# MK64 Reloaded

This is an HD texture pack for Mario Kart 64 for GLideN64 + Recomp and [Dolphin](https://github.com/GhostlyDark/MK64-Reloaded-Dolphin) and [SpaghettiKart](https://github.com/GhostlyDark/MK64-Reloaded-SK).

![](/mk64-reloaded.jpg)

# Install

## [Project64](https://www.pj64-emu.com/windows-downloads) using [latest GLideN64 WIP build](https://github.com/gonetz/GLideN64/releases)

1. Press the "Code button" on the right side of the Github page, then "Download .ZIP".
2. Once downloaded, extract everything that's inside of the ZIP into your `~/Project64/Plugin/GFX/GlideN64/hires_texture/MARIOKART64` folder.[^paths]
3. Make sure the game runs, then adjust the graphics configuration for your Mario Kart 64 rom by highlighting the game in your ROM Directory within P643.0, then:
4. Options > Configuration > Config: Mario Kart 64: Plugins > Video > GlideN64.
5. Options > Graphics Settings > Texture Enhancement > Check "Use Texture Pack" and "Use file storage instead of memory cache" and point file paths to the texture pack.

## [Mupen64Plus](https://www.mupen64plus.org) using [latest GLideN64 WIP build](https://github.com/gonetz/GLideN64/releases)

1. Press the "Code button" on the right side of the Github page, then "Download .ZIP". If you are using [RMG](https://github.com/Rosalie241/RMG/releases), instructions are similar to the ones of Project64.
2. Once downloaded, extract everything that's inside of the ZIP into your `%APPDATA%/Mupen64Plus/hires_texture/MARIOKART64` folder.
   - On Linux, the path is: `~/.local/share/mupen64plus/hires_texture`
   - On macOS, the path is: `~/Library/Application Support/Mupen64plus/hires_texture`
3. Edit the config file found in `%APPDATA%/Mupen64Plus`
   - On Linux, the path is: `~/.config/mupen64plus`
   - On macOS, the path is: `~/Library/Application Support/Mupen64plus`
4. Set the parameter `LoadHiResTextures` and `txHiresTextureFileStorage` to `True`. [^cache]

## [Retroarch](https://www.retroarch.com)

**Use the Mupen64Plus-Next core.**

1. Press the "Code button" on the right side of the Github page, then "Download .ZIP".
2. Once downloaded, put everything that's inside of the ZIP into your `~/RetroArch-Win64/System/Mupen64plus/hires_texture/MARIOKART64` folder.
3. Ensure that the `cache` folder exists in the directory.
3. From the Retroarch main menu, go to Load Core > Download a Core > Nintendo - Nintendo 64 (Mupen64Plus-Next).
   - Android users need the Mupen64Plus-Next GLES3 core.
4. Load the target rom, then access the Quick Menu > Options > GlideN64 > Use High-Res textures
   - Also enable:
     * Cache Textures
     * Use High-Res Full Alpha Channel
     * Use Hi-Res Storage
