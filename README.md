[Sizer]: https://www.brianapps.net/sizer/
[Brian Apps]: https://www.brianapps.net/
[systray]: https://www.brianapps.net/sizer/userguide.html#systray
[screenshot]: https://github.com/kenkin360/Sizer-Xfce4/blob/main/images/captrue.jpg
[Sizer for Xfce 4]: https://github.com/kenkin360/Sizer-Xfce4

# Sizer for Xfce 4

![screenshot][screenshot]

This project is an Xfce4 tool inspired by [Sizer] which allows users resize/move windows in a few clicks. 

[Sizer for Xfce 4] attempts to bring similar functionality to the Xfce desktop.

## Requirements
The following dependencies are required: 
- `yad`
- `xdotool`

To install them on Debian/Ubuntu-based systems:
```bash
sudo apt install yad xdotool
```
Or use the corresponding installation command on other Linux distros.

## Installation
1. Clone the repository

```bash
git clone https://github.com/kenkin360/Sizer-xfce4
```

2. On the Xfce panel:

 - Right-click → **Panel** → **Add New Items**
 - Select **Launcher**
 - In the Launcher properties, **Add a new empty item**, and set its **Command** to point to the **[Sizer-xfce4](https://github.com/kenkin360/Sizer-xfce4/blob/main/Sizer-xfce4)** script.
 - You might want to pick a distinctive icon(a crosshair, maybe) to make it easy to recognize.

## Usage
- This project implements functionality similar to the [System Tray Resizing][systray] feature of [Sizer]. 
- Because it is integrated through the Xfce Panel Launcher, the selection menu appears on **left-click** of the icon. 
- It cannot replace the panel's right-click behavior due to Xfce panel design restrictions.
- Configuration is loaded from a `.reg` file follows [Sizer] registry format. 
- To create or modify presets, you may either export the registry key with **regedit** or create it manually. The expected key is:
```
[HKEY_CURRENT_USER\Software\Sizer]
```

## Disclaimer
- This project has only been tested on **Xfce 4**. It may work on other Linux desktop environments, but users will need to test on their own.
- This project is an independent utility and is not affiliated with [BrianApps], the original [Sizer], nor is it part of the official Xfce project.

## License
MIT
