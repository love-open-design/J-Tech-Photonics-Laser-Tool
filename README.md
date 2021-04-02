# XY Plotter Tool by Love Open Design

This is the official repository for the XY Plotter Tool Inkscape extension.

## Purpose

This extension work for the [DIY XY Plotter High Precision Drawbot](https://www.aliexpress.com/item/32917861259.html?spm=a2g0s.9042311.0.0.3d9f6c37xpT5iS) on Ali Express

## Installation

Download the latest release [here](https://github.com/love-open-design/XY-Plotter-Tool-by-LOD/release). Make sure to select the release targeted towards the version of Inkscape you are using. You can find the version of Inkscape you're using under **Help** > **About**.

Unzip the files directly into the Inkscape user extensions folder. Inkscape lists the location of your extensions folder under **Edit** > **Preferences** > **System**.

Restart Inkscape and you're done.

## Documentation

## Basic command

* Pen Up: `M5 S0`
* Pen Down: `M3 S1000`
* Pen Delay: `P4 P<your delay ms>`
* Pen Speed Movement: `G1 F<your speed>`

### Custom G-code Header and Footer

Add "header" and "footer" text files without extensions in your destination directory to add custom commands. Don't forget to add a new line at the end of these two files.

If no files are detected the default values are :
- Header : G90 ; Absolute positioning
- Footer : G1 X0 Y0 ; Move to X0 Y0

## For developers

Pull requests are welcome. Just make sure to test your code on both Python >=2.6 and >=3.5 for the main branch, and Python >= 3.6 for the development branch (In the next major release we'll drop support for older python versions in an effort to improve code readability).

## Credits

This inkscape extension is adapted from [J-Tech-Photonics-Laser-Tool](https://github.com/JTechPhotonics/J-Tech-Photonics-Laser-Tool) inkscape extension.
