#!/bin/bash

cat << 'EOF' > README.md
# Windows 11: My take on "Ricing"

This repository is a backup of my personal Windows 11 configuration. The goal of this setup is stripping away the "Windows bloat" and building a keyboard-centric environment that removes non-essential-ness out of the way until I need it. 

I believe a workspace should be organised and efficient. If an element doesn't serve a mechanical purpose, I hide it.

---

## 🖥️ UI & Aesthetics

*   **Segmented Floating Taskbar**: Instead of a solid bar, each icon lives in its own floating black box. It’s physically separated from the system tray to create a cleaner, modular look.
*   **The "Start-less" Workflow**: I’ve hidden the Windows Start button. If the only point is to search for apps, a dedicated button is just wasted space.
*   **Custom Typography**: I changed the File Explorer font to **JetBrains Mono**. It’s much cleaner than the stock Windows fonts and fits a developer-focused aesthetic.
*   **Minimalist System Tray**: I hid everything I don't use. Only the essentials—WiFi, the system tray, and a custom clock—remain.
    *   Modified to show `24h:min Day, Mon Date`.

---

## ⌨️ Navigation & Shortcuts

I prefer keeping my hands on the keyboard as much as possible.

*   **Numbered Taskbar**: Apps are numbered so I can jump between them instantly using `Win + [Number]`.
*   **Desktop Indicators**: Those small dots on the far right act as workspace indicators. I use multiple desktops to stay organised without having to `Alt + Tab` through twenty windows on a single screen.
*   **Window Management**:
    *   `Win + Q` and `Win + S` are turned off. 
    *   `Win + Q` has been rebound to **ALT + F4** using external application(s). 
    *   `Alt + Shift + Num`: Instantly moves a window to a specific desktop (e.g., tossing Discord or WhatsApp to desktop 3).
*   **No Copilot**: I disabled `Win + C` because I don’t use it.

---

## 🛠️ The Fixes

Windows has some native quirks that I’ve used **Windhawk** to resolve:

*   **Taskbar Order**: In stock Windows, apps will rearrange themselves when you switch virtual desktops. I use a mod to ensure they remember their latest locations.
*   **Centred Action Centre**: When I hit `Win + A`, the menu now pops up in the centre of the screen instead of the corner.

---

## 📦 What’s in this Repo?

*   `windhawk_mods.reg`: A full export of my active mods and their enabled states.
*   `custom_windows_taskbar.json`: The specific JSON logic for the segmented, floating taskbar boxes.
*   `custom_windows_taskbar_for_copy.json`: The same file, but in one long line for pasting in Windhawk.
*   `assets/`: Screenshots and previews.

---

## 🚀 Setup

1.  Install **Windhawk**.
2.  Make sure **JetBrains Mono** is installed.
3.  Import the `.reg` file or copy the JSON from `custom_windows_taskbar.json` into the **Taskbar Styler** advanced settings.
4.  Set the File Explorer font to **JetBrains Mono**.
EOF# Windows-11-windhawk-ricing
