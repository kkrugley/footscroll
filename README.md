[![Build and Release](https://github.com/kkrugley/footscroll/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/kkrugley/footscroll/actions/workflows/build.yml)
![Static Badge](https://img.shields.io/badge/ZMK_Firmware-blue?style=flat&logo=qmk)
![Static Badge](https://img.shields.io/badge/AutoHotkey-v2-green?style=flat&logo=autohotkey)



# FootScroll: Foot Pedal for Scrolling

FootScroll is a concept and prototype of a foot pedal designed for controlling video content scrolling (TikTok, YouTube Shorts, Reels).

## Concept
Reimagining the sewing machine foot pedal. Back then - a tool that freed hands for work. Now - frees hands to avoid work.

One gesture - scroll. Only forward. Dumb scrolling doesn't imply going back.

## Hardware
*   **Controller:** nice!nano (BLE HID)
*   **Power:** Li-ion battery
*   **Case:** 3D-printed plastic case from 3 parts
*   **Interfaces:** 1 USB Type-C port - shared for charging and flashing, 2 switches - one for mode switching, one for power on/off

## Software

### Windows

*   **Script:** `footscroll_setup.ps1` (includes installing AutoHotKey v2, defining monitor coordinates, and AHK script).
*   **Logic:** Pedal press (F14) → AHK intercepts input → cursor teleports to second monitor → scrolling → cursor return.


### iPad

*   **Logic:** Pedal press emulates rapid mouse wheel scrolling (Burst scrolling).