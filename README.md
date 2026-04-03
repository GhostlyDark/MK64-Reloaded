# MK64 Reloaded

MK64 Reloaded is an HD texture pack for GLideN64, rt64 (Recomp), Dolphin and SpaghettiKart.

> [!IMPORTANT]
> Release files can be found over at [evilgames.eu](https://evilgames.eu/texture-packs/mk64-reloaded.htm) and [GitHub Releases](https://github.com/GhostlyDark/MK64-Reloaded/releases/latest).

![](/mk64-reloaded.jpg)



## Porting scripts

> [!Tip]
> This repository contains scripts for automated porting of textures to supported platforms. They require bash v4 and a native Linux environment. On Windows, it is recommended to use WSL2 from within the `wsl.localhost` file system. The scripts will also work using MSYS2, but file operations are going to run much slower. Currently available are `dolphin.sh` and `spaghetti.sh`.

Make script executable and run it:

```
chmod u+x dolphin.sh
```

```
./dolphin.sh
```

Ported files will be available inside `_build`.



## Texture rescaling

The `mk64.tdb` file contains information about the original texture sizes, which can be used by [Bighead's Custom Texture Tool](https://forums.dolphin-emu.org/Thread-custom-texture-tool-ps-v52-5) to rescale them to a new upscale ratio. This way, an HD replacement for a 32x32 texture can be rescaled to 8x the original resolution (256x256), down from however big the given HD texture might be.



## GLideN64

> [!NOTE]
> Latest [WIP build](https://github.com/gonetz/GLideN64/releases/github-actions) required. Use `PJ64Legacy-Qt-x86` if Project64 is your emulator of choice.

Pre-compiled `.hts` files are `cache` files and have to be located inside:

- Project64: `Project64/Plugin/GFX/cache`
- RMG: `RMG/Cache/cache`
- mupen64plus:
-- Windows: `%appdata%/mupen64plus/cache`
-- Linux: `~/.cache/mupen64plus/cache`
-- macOS: `~/Library/Application Support/Mupen64plus/cache`
- mupen64plus-nx (RetroArch): `RetroArch/system/Mupen64plus/cache`


**Only for advanced users:** HTS cache can be generated from the source PNG textures:

- Project64: `Project64/Plugin/GFX/hires_texture/MARIOKART64`
- RMG: `RMG/Data/hires_texture/MARIOKART64`
- mupen64plus:
-- Windows: `%appdata%/mupen64plus/hires_texture/MARIOKART64`
-- Linux: `~/.local/share/mupen64plus/hires_texture/MARIOKART64`
-- macOS: `~/Library/Application Support/Mupen64plus/hires_texture/MARIOKART64`
- mupen64plus-nx (RetroArch): `RetroArch/system/Mupen64plus/hires_texture/MARIOKART64`


Required graphics settings (named differently depending on emulator):

- Set texture pack usage: `Use texture pack` | `txHiresEnable` | `Use High-Res textures` to **On**
- Set use of full alpha: `Use full transparencies` | `txHiresFullAlphaChannel` | `Use High-Res Full Alpha Channel` to **On**
- Set use of HTS over HTC: `Use file storage instead of memory cache` | `txHiresTextureFileStorage` | `Use enhanced Hi-Res Storage` to **On**


Optional (but recommended) settings:

- Set cache compression: `Compress texture cache` | `txCacheCompression` | `Use High-Res Texture Cache Compression` to **Off**
- Fix black lines: `Fix black lines between 2D elements: For adjacent 2D elements` | `CorrectTexrectCoords: 1 (Auto)` | `Continuous texrect coords: Auto`
- Use `8x multiple of N64 resolution` or lower
- mupen64plus-nx (RetroArch): `INI Behaviour: Prioritize Core Options over INI`



## Dolphin

> [!NOTE]
> Download a recent [release build](https://dolphin-emu.org/download). DDS textures for playing are highly recommended.

- Click `File --> Open User Folder` and copy the texture folder into `Load/Textures`
- Open `Graphics --> Advanced` and activate `Load Custom Textures`



## SpaghettiKart

> [!NOTE]
> O2R files go into the `mods` directory.

Released texture files are packaged into a `.zip` file with the file extension changed to `.o2r`. It's recommended to use `0 - Store` as in no compression for best performance. SpaghettiKart accepts mods packaged into an `.o2r`, `.zip` or simply as a folder, each containing the `textures` directory and `mods.toml`. Refer to [modding.md](https://github.com/HarbourMasters/SpaghettiKart/blob/main/docs/modding.md), [mods-toml.md](https://github.com/HarbourMasters/SpaghettiKart/blob/main/docs/mods-toml.md) and [texture-packs.md](https://github.com/HarbourMasters/SpaghettiKart/blob/main/docs/textures-pack.md) for more details.



## rt64 (MarioKart64Recomp)

Download the `.rtz` file. Launch the game and go into the mods menu. You may drop the file on top of the game window or use the `Install Mods` button.



## Credits

Contributors:

- Admentus
- Aghanim
- amxr
- Andrat
- AndresL64
- Darth-Koopa
- DinkyDIC
- Dokotroopi
- Fanamel
- GhostlyDark
- katherinecode
- kette
- Matteoki
- Nerrel
- PaichnidiGCN
- PokeHeadroom
- Retro64
- Sign
- Sunset
