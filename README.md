[English](README.md) · [Українська](README.uk.md) · [Русский](README.ru.md)

🌐 All our programs: https://drugoj00.github.io/

# Phone in Window with Sound

Shows the real screen of an Android phone in a window on a Windows PC. You can click with the mouse, type on the keyboard and listen to the phone's sound through the computer. Apps keep running on the phone itself; the computer only shows the screen and sends your input, so banking apps, messengers and everything else behave as usual.

⭐ If the program is useful, please star this repository: it costs nothing and helps other people find it.

## Download

**Current version: 1.0.** **[Latest version: PhoneInWindowWithSound-1.0.exe](https://github.com/drugoj00/phone-in-window-with-sound/releases/latest)** (Assets section). [All versions](https://github.com/drugoj00/phone-in-window-with-sound/releases).

The installer is about 31 MB: scrcpy with audio is already inside, so you don't need the internet to install, and administrator rights are optional. The SHA-256 checksum of the file is listed in the description of each release. The installer works on Windows 10 and 11. The program is available in English, Ukrainian and Russian and picks the language from your Windows language.

## Features

- Mouse and keyboard: a click works as a tap, the wheel scrolls, and you can type straight into the phone's text fields.
- Phone sound on the computer: Android 11 and newer out of the box, Android 10 through the small sndcpy app (installed automatically). There is no sound on Android 9 and older.
- Six buttons beside the window: Copy, Paste (text in any language), Rotate, Turn off screen (turns off the phone's screen), Tools and About / Support. In a portrait window they sit in a vertical strip to the right of the window (in the colour of its title bar), in landscape in the title bar. The window opens in the same orientation as the connected phone.
- Tools menu: screenshot, screen recording with sound, phone files (download and send), apps (launch, stop, uninstall), install APK, connect over Wi-Fi in one click (the phone is remembered). You can also drag an .apk file onto the phone window: the app gets installed; any other file goes to the phone's "Download" folder.
- The phone does not fall asleep or lock while the window is open; the picture and sound don't drop out.
- Several phones at once: each gets its own window, and the "Windows (all)" shortcut opens all connected phones.
- Connection by cable, by Wi-Fi after connecting once with a cable, and by Wi-Fi without a cable on Android 11 and newer.
- Phone report: the program collects information about the phone (serial numbers and addresses are hidden) and tells you what to turn on.
- A detailed guide and a "Check for updates" option for scrcpy are built into the program.

## Screenshots

![The six buttons: in a portrait window in a strip beside the window, in landscape in the title bar.](https://drugoj00.github.io/phone-in-window-with-sound/buttons_en.png)

![The Tools menu.](https://drugoj00.github.io/phone-in-window-with-sound/tools_en.png)

![The About window.](https://drugoj00.github.io/phone-in-window-with-sound/about_en.png)

## Getting started

1. Run the installer.
2. On the phone, turn on Developer options once (Settings, About phone, tap "Build number" 7 times) and "USB debugging".
3. Connect the phone with a cable, allow debugging ("Allow USB debugging?") and launch the "Window (cable)" shortcut.

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
