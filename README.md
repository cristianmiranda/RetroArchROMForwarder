# RetroArch ROM Forwarder

Based on [https://github.com/The-4n/hacBrewPack](https://github.com/The-4n/hacBrewPack) with a few perks to make it easier to use and ready for macOS.

## Installation

    git clone https://github.com/cristianmiranda/RetroArchROMForwarder.git
    cd RetroArchROMForwarder
    npm i

## Requisites

1.	Get prod.keys using [Lockpick RCM](https://github.com/shchmue/Lockpick_RCM) ([Lockpick](https://github.com/shchmue/Lockpick) might not be enough).
2.	Use 256x256 images. Not sure what happens if resolution is not exactly that.
3.	Feel free to replace 'hacbrewpack' with your own compiled version. This one is v3.05.
4.	Install Node JS to use this tool.

## Usage

	  # -t | --titleName   : Title Name
	  # -c | --coreNroPath : RetroArch Core NRO path inside SD card (sdmc:)
	  # -r | --romPath     : RetroArch ROM path inside SD card (sdmc:)
	  # -i | --imagePath   : Game image path. Must be 256x256
	  # -k | --keysPath    : Switch keys path. Use Lockpick RCM
	  # -o | --outputPath  : Generated NSP file path

    node RetroArchROMForwarder.js -t 'Pokemon - Emerald Version' -k prod.keys -c '/retroarch/cores/mgba_libretro_libnx.nro' -r '/retroarch/roms/Nintendo - Game Boy Advance/Pokemon - Emerald Version.gba' -o ~/Desktop/. -i ~/Downloads/poke.jpg


## Original hacBrewPack usage (clone repo first)

    cd RetroArchROMForwarder
    ./hacbrewpack --titleid 0527D4338C310000 --titlename 'Pokemon - Emerald Version' --titlepublisher Nintendo


## Useful links
* [Lockpick RCM](https://github.com/shchmue/Lockpick_RCM)
* [https://github.com/The-4n/hacBrewPack](https://github.com/The-4n/hacBrewPack)
* [https://devkitpro.org/wiki/devkitPro_pacman](https://devkitpro.org/wiki/devkitPro_pacman)
* [elf2nso](https://git.m4xw.net/Switch/RetroArch/libnx/blob/4a371f441735ec1008b91dc0a0e2f2e00168d65b/tools/Makefile)
* [https://brewinstall.org/Install-lz4-on-Mac-with-Brew/](https://brewinstall.org/Install-lz4-on-Mac-with-Brew/)
* [Generate RetroArch NSP Forwarders (with proper icon and title)](https://gbatemp.net/threads/generate-retroarch-nsp-forwarders-with-proper-icon-and-title.528775/)
* [RetroArch NSP Forwarder mod](https://github.com/natinusala/nx-hbloader-retroarch-forwarder-mod)
* [https://github.com/Root-MtX/Nro2Nsp](https://github.com/Root-MtX/Nro2Nsp)
