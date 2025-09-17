# XFCE4 Sizer (Unofficial)

![screenshot](https://github.com/kenkin360/Sizer-xfce4/blob/main/images/captrue.jpg)

This project is an XFCE4 tool inspired by [Sizer](https://www.brianapps.net/sizer/).  
Sizer on Windows allows users to quickly resize windows to specific dimensions.  
This project attempts to bring similar functionality to the XFCE desktop.

## Features
- Predefined window sizes (e.g. 800×600, 1024×768, 1920×1080)
- One-click resizing of the currently active window
- Lightweight, no background daemon
- Integrates with the XFWM4 window manager

## Requirements
Please install the following dependencies:
- `yad`
- `xdotool`

On Debian/Ubuntu-based systems:
```bash
sudo apt install yad xdotool
```

## Installation & Usage
1. Place the script from this project in any directory you prefer (e.g. `~/xfce4-sizer/`).  
2. On the XFCE panel:  
   - Right-click → **Panel** → **Add New Items**  
   - Select **Launcher**  
   - In the Launcher properties, **Add a new empty item**, and set its command to point to the script.  
3. Once added, click the panel icon, select a size, and the active window will be resized.

## Notes
- This project has only been tested on **XFCE4**.  
- It may work on other Linux desktop environments, but users will need to test on their own.  
- This project is not affiliated with BrianApps or the original Sizer.

## License
MIT
