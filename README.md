# Lenovo Ideapad battery conservation mode on GNU/Linux
[![made-with-bash](https://img.shields.io/badge/Made%20with-Bash-1f425f.svg)](https://www.gnu.org/software/bash/)
[![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
[![HitCount](https://hits.dwyl.com/tildehacker/ideapad-conservation-mode.svg)](https://hits.dwyl.com/tildehacker/ideapad-conservation-mode)
[![start with why](https://img.shields.io/badge/start%20with-why%3F-brightgreen.svg)](https://tildehacker.com/lenovo-ideapad-battery-conservation-mode-gnu-linux)

<video autoplay loop muted playsinline>
	<source src="ideapad-cm-screencast.webm" type="video/webm">
	<source src="ideapad-cm-screencast.mp4" type="video/mp4">
</video>

A script to enable/disable battery conservation mode in Lenovo Ideapad laptops. :computer: :battery: :guardsman:

## Motivation

When the conservation mode is enabled, your battery will only be charged to 60%
to maximize its lifespan. On Windows, [Lenovo
Vantage](https://techtoday.lenovo.com/us/en/software/vantage) is usually used to
enable this mode. On GNU/Linux, this can be
[done](https://tildehacker.com/lenovo-ideapad-battery-conservation-mode-gnu-linux)
manually. This script is a shortcut to enable/disable this mode.

## Installation (Arch User Repository)

`ideapad-cm` is available in the [Arch User Repository
(AUR)](https://aur.archlinux.org/packages/ideapad-cm). The following command
installs `ideapad-cm` using [`yay`](https://github.com/Jguer/yay) AUR helper.

```bash
yay -S ideapad-cm
```

## Installation (Arch Linux)

If you use Arch Linux, then you can use the bundled PKGBUILD file to build and
install this script.

```bash
git clone https://github.com/tildehacker/ideapad-conservation-mode.git
cd "ideapad-conservation-mode"
makepkg
sudo pacman -U *.tar.xz
```

## Installation
Clone this repository to a directory of your choice and add it to your PATH environment variable.

### Clone
```bash
git clone https://github.com/tildehacker/ideapad-conservation-mode.git
```

### Add it to PATH
Adjust `.bashrc` according to your current shell.
```bash
echo "export PATH=\$PATH:$( pwd )" >> ~/.bashrc
```

## Usage
```bash
Usage:
	ideapad-cm enable|disable|status [acpi_call|ideapad_laptop]
```

## Contributing [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://makeapullrequest.com)
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
This project is licensed under the GPL-3.0 License - see the [LICENSE](LICENSE)
file for details.
