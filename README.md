[English](README.md) · [Українська](README.uk.md) · [Русский](README.ru.md)

🌐 All our programs: https://drugoj00.github.io/

<img src="https://drugoj00.github.io/phone-in-window-with-sound/icon.png" alt="" width="96" align="right">

# Phone in Window with Sound

Shows the real screen of an Android phone in a window on a Windows PC. You can click with the mouse, type on the keyboard and listen to the phone's sound through the computer. Apps keep running on the phone itself; the computer only shows the screen and sends your input, so banking apps, messengers and everything else behave as usual.

⭐ If the program is useful, please star this repository: it costs nothing and helps other people find it.

## Download

**Current version: 1.5.** **[Latest version: PhoneInWindowWithSound-1.5.exe](https://github.com/drugoj00/phone-in-window-with-sound/releases/latest)** (Assets section). [All versions](https://github.com/drugoj00/phone-in-window-with-sound/releases).

The installer already contains scrcpy with audio, so you don't need the internet to install, and administrator rights are optional. The SHA-256 checksum of the file is listed in the description of each release. The installer works on Windows 10 and 11. The program is available in English, Ukrainian and Russian and picks the language from your Windows language.

## What is new in version 1.5

- Tooltip on every button.
- Denser menus and drop-down lists, like Windows; a drawn check mark on checked items in the dark theme.
- Program texts without first person.
- The “By cable” and “Over Wi-Fi” lists and the device picker: set-top boxes on the local network are found automatically.
- In the lists and the picker: name, model, connection (USB cable, wired LAN, Wi-Fi) and address; “Rename…” button.

## What is new in version 1.4

- Fixed: screen timeout is left alone while the phone is charging.
- Fixed: rotation on Android 10 (A7, S9), including apps that lock their orientation.
- Fallback rotation method for Android 9 and older.
- Fixed: the “Screen timeout” list shows the real timeout.

## What is new in version 1.3

- Install APK, APKS, APKM, XAPK, ZIP with OBB: “Install app…” and drag-and-drop onto the window.
- “Start Shizuku from the PC” button.
- Tray: “Skip in “All phones” mode”.
- “About”: “All our programs” link.
- “Keep the screen on while the window is open” switch.
- Fixed: second icon on Samsung (“Dual app”) when installing an APK.
- Fixed: screen timeout is no longer overwritten when the window closes.
- Fixed: rotation: a leftover “ignore app orientation” is removed only if the program itself enabled it.

## What is new in version 1.2

- A serious phone-rotation bug is fixed. On some phones (seen on the Samsung Galaxy A14) the “ignore app orientation” mode, a locked rotation and a switched-off auto-rotate could stay behind after the window was used: the screen “glitched” or lay in landscape even though the window was already closed. Now the return of the previous settings is verified: the program reads them back from the phone and repeats the return (3 attempts, then up to 10 more minutes if the phone is busy or unreachable), and the safety record is kept until the return is confirmed. A leftover “ignore app orientation” mode without our record is removed automatically when the program starts, when a window opens and after it closes; when the program exits it makes a last attempt to restore the settings.
- If a phone already has such a glitch: connect it and start the program, the “ignore app orientation” mode will be removed by itself. If auto-rotate is off, switch it on in the phone's quick settings.

## What is new in version 1.1

- The Tools menu has a new “ADB tools” submenu: “ADB commands” (a separate button in the icon strip and a menu item; a command box, history, ready-made commands; reboot, recovery, bootloader and power off with confirmation), “Device information” (Android, battery, memory, screen, Wi-Fi address), “Quick settings” (brightness, screen timeout, stay awake while charging, animations, volume, DPI, Wi-Fi and mobile data), “Phone log” (logcat with a filter and saving to a file), “Keys and input” (Back, Home, Recents, volume, typing text, opening a link on the phone).
- The “Apps” window shows the size and install/update dates of every app, sorts by size and date, can show real app icons (the “Icons” tick, off by default), has a row of “Show” buttons (user, system, disabled, removed, all), selecting several apps with batch removal and batch APK installation (also by dragging onto the window), and can show system apps, disable and re-enable apps (protected system apps cannot be disabled), view and change an app’s permissions, clear its data and save its APK to the computer.
- Missing Android drivers are installed automatically from the internet (the Microsoft catalog): if the phone is not visible but an Android device without a driver is present, the program downloads and installs the driver by itself (Windows asks for administrator permission once); it can also be started by hand: Tools → ADB tools → Android drivers.

## Features

- Mouse and keyboard: a click works as a tap, the wheel scrolls, and you can type straight into the phone's text fields.
- Phone sound on the computer: Android 11 and newer out of the box, Android 10 through the small sndcpy app (installed automatically). There is no sound on Android 9 and older.
- Six buttons beside the window: Copy, Paste (text in any language), Rotate, Turn off screen (turns off the phone's screen), Tools and About / Support. In a portrait window they sit in a vertical strip to the right of the window (in the colour of its title bar), in landscape in the title bar. The window opens in the same orientation as the connected phone.
- Tools menu: screenshot, screen recording with sound, phone files (download and send), apps (launch, stop, uninstall), install APK, connect over Wi-Fi in one click (the phone is remembered). You can also drag an .apk file onto the phone window: the app gets installed; any other file goes to the phone's "Download" folder.
- The phone does not fall asleep or lock while the window is open; the picture and sound don't drop out.
- Several phones at once: each gets its own window, and the "All" button in the "Phone in Window" panel opens all connected phones.
- One shortcut and a tray icon: the "Phone in Window" shortcut opens a panel (By cable, Over Wi-Fi, Android 11 and newer, All); each button opens a list of matching phones beside the window. The icon stays in the tray: a click hides or shows the window, closing the window does not remove the icon, and the program can start with Windows in the tray without a window. Language (English, Ukrainian, Russian) and theme (auto, light, dark) are chosen in the panel.
- Connection by cable, by Wi-Fi after connecting once with a cable, and by Wi-Fi without a cable on Android 11 and newer.
- Phone report: the program collects information about the phone (serial numbers and addresses are hidden) and tells you what to turn on.
- A detailed guide and a "Check for updates" option for scrcpy are built into the program.

## Screenshots

![The launcher window: the connection buttons, language and theme.](https://drugoj00.github.io/phone-in-window-with-sound/launcher_en.png)

![The six buttons: in a portrait window in a strip beside the window, in landscape in the title bar.](https://drugoj00.github.io/phone-in-window-with-sound/buttons_en.png)

![The Tools menu.](https://drugoj00.github.io/phone-in-window-with-sound/tools_en.png)

![The About window.](https://drugoj00.github.io/phone-in-window-with-sound/about_en.png)

## Getting started

1. Run the installer.
2. On the phone, turn on Developer options once (Settings, About phone, tap "Build number" 7 times) and "USB debugging".
3. Connect the phone with a cable, allow debugging ("Allow USB debugging?") and open the "Phone in Window" shortcut and click "By cable".

## Requirements

- Windows 10 or 11.
- An Android 5.0 or newer phone (copy and paste work from Android 7).
- A cable that carries data, not just charge.

## Limitations

- iPhone is not supported.
- Xiaomi, Redmi and POCO phones need "USB debugging (Security settings)" turned on, otherwise the mouse and keyboard won't work.
- Some banking apps don't like "USB debugging" being on and may refuse to open: that is up to the app itself.
- Phone calls and apps that forbid recording their sound can't be heard in the window.
- Tested on Samsung Galaxy S9, A7 and A14.
- The installer is not signed with a publisher certificate yet, so Windows may show a SmartScreen warning ("unknown publisher"): click "More info" and then "Run anyway" if you downloaded the file from here.

## What it is made of

- [scrcpy](https://github.com/Genymobile/scrcpy) (Genymobile, Apache 2.0 license): shows the screen and passes your clicks and keystrokes to the phone.
- [sndcpy](https://github.com/rom1v/sndcpy) (Romain Vimont, Apache 2.0 license): forwards the sound from Android 10.
- The wrapper (launcher, phone selection, window buttons, rotation, sound for Android 10, installer, phone report) is written separately and is not a Genymobile product.

## News and support

- Telegram channel: [t.me/PhoneInWindowSound](https://t.me/PhoneInWindowSound)
- Website: [drugoj00.github.io/phone-in-window-with-sound](https://drugoj00.github.io/phone-in-window-with-sound/)

## Support the project

The program is free. If it is useful to you, you can support its development by card, Google Pay or USDT. For USDT use the TRON (TRC20) network only (coins sent through another network are lost).

- By card or Google Pay (any amount from 50 UAH): https://secure.wayforpay.com/button/bba92579a4647

USDT (TRON/TRC20):

```
TXk32CLkwJryTqhmkw6urcM5CacJgPsSpJ
```
