# LibreSprite [![Liberapay](https://i.imgur.com/UOLKpPA.png "Support our work")](https://liberapay.com/LibreSprite/)
[![Linux](https://github.com/LibreSprite/LibreSprite/actions/workflows/cmakeLinux.yml/badge.svg)](https://github.com/LibreSprite/LibreSprite/actions/workflows/cmakeLinux.yml) [![Windows x64](https://github.com/LibreSprite/LibreSprite/actions/workflows/cmakeWin64.yml/badge.svg?branch=master)](https://github.com/LibreSprite/LibreSprite/actions/workflows/cmakeWin64.yml) [![MacOS](https://github.com/LibreSprite/LibreSprite/actions/workflows/cmakeMacOs.yml/badge.svg)](https://github.com/LibreSprite/LibreSprite/actions/workflows/cmakeMacOs.yml) [![Android](https://github.com/LibreSprite/LibreSprite/actions/workflows/cmakeAndroid.yml/badge.svg)](https://github.com/LibreSprite/LibreSprite/actions/workflows/cmakeAndroid.yml)

## Introduction
LibreSprite is a free and open source program for creating and animating your sprites.
* Real-time animation previews.
* Onion skinning.
* Multiple sprites can be edited at once.
* Ready to use palettes, or make your own.
* Sprites are composed of both layers & frames.
* Tiled drawing mode, useful to draw patterns and textures.
* Pixel precise tools like filled contour, polygon, shading mode, etc.
* Several file types supported for your sprites and animations.

## ZX Spectrum Support
LibreSprite includes a powerful, built-in `.asm` exporter specifically designed for ZX Spectrum homebrew development. 
- **Automatic 8x8 Block Grid:** Your image is automatically divided into standard 8x8 pixel blocks during export.
- **Ink and Paper Detection:** You don't need to manually configure Ink or Paper colors. The exporter counts the colors used in each 8x8 block. The most used color becomes the **Paper** (background), and the second most used becomes the **Ink** (foreground). 
- **Automatic Color Clash:** If you use more than 2 colors inside the same 8x8 block, the exporter will automatically preserve the two most used colors and assign the remaining pixels to the Paper color, perfectly simulating the classic ZX Spectrum Color Clash hardware limitation.
- **Nearest Color Matching:** No matter what RGB colors you draw with, the exporter will automatically convert every pixel to the closest hardware color from the official 15-color ZX Spectrum palette.
- **Sprite Deduplication:** Repeated 8x8 blocks are deduplicated to save memory, producing a highly optimized `map_array` and individual sprite definitions ready for `ZXSpriter` or your own game engine!

## Download
Get the [latest release](https://github.com/LibreSprite/LibreSprite/releases/latest) for Linux, MacOS, Windows or Android.

## History
LibreSprite originated as a fork of [Aseprite](https://www.aseprite.org), developed by [David Capello](https://github.com/dacap). Aseprite used to be distributed under the GNU General Public License version 2, but was moved to a proprietary license on [August 26th, 2016](https://github.com/aseprite/aseprite/commit/5ecc356a41c8e29977f8608d8826489d24f5fa6c).

This fork was made on the [last commit](https://github.com/aseprite/aseprite/commit/03be4aa23db465219962f4c62410f628e7392545) covered by the GPL version 2 license, and is now developed independently of Aseprite.

## Contributing
As LibreSprite has a newly budding community, we need help building the infrastructure of our development, support, and news networks. If you would like to help, please make yourself known at our [Discord](https://discord.gg/95gbyU5) or [Matrix](https://matrix.to/#/%23libresprite:matrix.org), and checkout our guide on [contributing](CONTRIBUTING.md).

## Compiling
Don't worry, it isn't as hard as you might think! Just follow the instructions [here](INSTALL.md).

## Theming
Don't like the default look of LibreSprite? Don't panic, you can download from the LibreSprite [resources](https://libresprite.github.io/#!/resources) repo. 

## License
This program is distributed under the [GNU General Public License Version 2](LICENSE.txt).

## Credits
An ***enormous*** thank you to the original developers of [Aseprite](https://www.aseprite.org), without them and their original licensing this project wouldn’t exist. Additional shout-outs are given in the [list of contributors](CONTRIBUTORS.md). If you have submitted work to LibreSprite and would like to have your name on the list, please create a pull request or get in touch and we’ll make it happen.
