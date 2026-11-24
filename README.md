# Varodex POS — till installers

The Windows till program for [Varodex](https://varodex-app.pages.dev). A till only works once it is paired with a
business: the pairing code comes from the Varodex back office (Settings → POS devices → Add till).

## Download

Open the **[newest version](https://github.com/varodex-app/varodex-pos-releases/releases/latest)** and, under
"Assets", download the file for your Windows:

| Windows | File name ends with |
|---|---|
| Windows 10 or 11 (64-bit) | `-win10-setup.exe` |
| Windows 7 or 8, or any 32-bit Windows | `-win7-setup.exe` |

Every version and what changed in it: [all releases](https://github.com/varodex-app/varodex-pos-releases/releases).

## Install

1. Download the installer for your Windows (above) and open it.
2. Windows may say "Windows protected your PC" (the installer is not signed yet): click **More info**, then
   **Run anyway**.
3. Choose where to install, then finish. A "Varodex POS" shortcut appears on the desktop.
4. Open it and type the pairing code from the back office.

## Updates

From version 1.2.1 the till updates itself: it downloads a new version in the background and installs it **only when
no shift is open**, so a sale is never interrupted. Sales not yet sent are kept and sent after the restart. Tills on an
older version (1.1.x) need the installer once, by hand.

## What is in this repository

Only the installers and the small update files the tills read (`latest.yml` for Windows 10/11, `win7.yml` for Windows
7/8), under Releases. The Varodex build publishes them automatically whenever the till's version changes. The program
does nothing without a pairing code from a Varodex business.
