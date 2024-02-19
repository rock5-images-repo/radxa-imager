# Radxa Imager
a customized version of rpi-imager with custom theme color, device name and logo for Radxa

![radxa imager screenshot](https://forum.radxa.com/uploads/default/original/2X/c/c8d8b1e9842cf1e8289f91d4df632cb51ea37ffc.png)

## Customizing rpi-imager

This repository contains a script named `patch-rpi-imager` that allows you to customize the Raspberry Pi Imaging Utility (`rpi-imager`) before building it from source.

## Usage

To use the `patch-rpi-imager` script, follow these steps:

This will apply your customizations to the rpi-imager source files.

The `patch-rpi-imager` script supports the following options:

- `--name`: Specify a custom name to replace "Raspberry Pi" with.
- `--color`: Specify a custom color theme.
- `--logo`: Specify the path to a custom banner logo image.
- `--app-icon`: Specify the path to a custom application icon image.
- `--logo-stacked`: Specify the path to a custom stacked logo image.
- `--app-icon-ico`: Specify the path to a custom .ico application icon image.
- `--app-icon-icns`: Specify the path to a custom .icns application icon image.

1. Clone or Download the upstream [rpi-imager](https://github.com/raspberrypi/rpi-imager)
```
git clone https://github.com/raspberrypi/rpi-imager.git
```

2. Run this script to apply patch, for example

```bash
./patch-rpi-imager --name "Apple Pie" --color "#ff0000" --logo "logo.png" --source "~/Downloads/rpi-imager"

3. Build rpi-imager:

Proceed with building the rpi-imager application as usual. Follow the build instructions provided in the rpi-imager repository.