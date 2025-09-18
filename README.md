![Sizer]: https://www.brianapps.net/Sizer/

![userguide]: https://www.brianapps.net/Sizer/userguide.html

![screenshot]: https://github.com/kenkin360/Sizer-xfce4/blob/main/images/captrue.jpg

# Sizer for xfce 4

![screenshot][screenshot]

This project is an XFCE4 tool inspired by [Sizer].
[Sizer] on Windows allows users to quickly resize windows to specific dimensions.
This project attempts to bring similar functionality to the XFCE desktop.

## Requirements
Please install the following dependencies:
- `yad`
- `xdotool`

On Debian/Ubuntu-based systems:
```bash
sudo apt install yad xdotool
```

## Installation
1. Clone the repository:

```bash
git clone https://github.com/kenkin360/Sizer-xfce4
```

2. On the XFCE panel:
 - Right-click → **Panel** → **Add New Items**
 - Select **Launcher**
 - In the Launcher properties, **Add a new empty item**, and set its **Command** to point to the **Sizer-xfce4** script. 

## Usage
- This project implements functionality similar to the [System Tray Resizing][userguide] feature of [Sizer]. 
- Because this tool is integrated through the XFCE Panel Launcher, the selection menu appears on **left-click** of the icon. 
- It cannot replace the panel's right-click behavior due to XFCE panel design restrictions.
- Configuration is loaded from a `.reg` file follows [Sizer] registry format. 
- To create or modify presets, you may either export the registry key with **regedit** or create it manully. The expected key is:
```
[HKEY_CURRENT_USER\Software\Sizer]
```

## Notes
- This project has only been tested on **XFCE4**.
- It may work on other Linux desktop environments, but users will need to test on their own.
- This project is not affiliated with BrianApps or the original [Sizer].

## License
MIT

