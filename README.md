# My-Cool-Keeb
# Name: Morning Star

An 81-key dual-layer custom mechanical keyboard powered by an RP2040 microcontroller and written in Rust using the RMK framework.

<img width="907" height="407" alt="Screenshot 2026-07-27 at 3 20 32 PM" src="https://github.com/user-attachments/assets/6d164fc4-4fd2-4e00-a6ca-6a284adbcded" />


---

## Overview & Why I made it

**Morning Star** is an 81-key custom mechanical keyboard designed for macOS and Windows.

I built Morning Star to build a personalized keyboard that I can use to its fullest as it has everything built around things I would need in my workflow. The Morning Star lets you control volume and brightness with rotary encoder controls, and custom macro triggers directly on the RP2040 hardware level.

---

## Main Features

* **Dual OS Layouts**: Dedicated **`mac`** (Layer 0) and **`win`** (Layer 1) modes with `MO(1)` layer switching and automatic modifier key swaps.
* **Dual Rotary Encoders**: Physical knobs dedicated to **System Volume** (`Vol Up / Down`) and **Display Brightness** (`Brightness Up / Down`).
* **Custom Hardware Macros**: 4 dedicated macro keys (`Macro1` – `Macro4`) for workflow shortcuts.
* **Optimized Switch Matrix**: 6x16 switch matrix running a 3ms debounce time for rapid input detection.

---

## 🗺️ Keymap Layouts

### Layer 0: Mac
```text
Escape   F1      F2      F3      F4      F5      F6      F7      F8      F9      F10     F11     F12     Macro1 Macro2 Macro3
Grave    1       2       3       4       5       6       7       8       9       0       Minus   Equal   Backsp Mute   Play/Pause
Tab      Q       W       E       R       T       Y       U       I       O       P       [       ]       \      _      _
Caps     A       S       D       F       G       H       J       K       L       ;       '       Enter   _      _      _
Shift    _       Z       X       C       V       B       N       M       ,       .       /       Shift   Up     _      _
MO(1)    Ctrl    Opt     Cmd     _       _       _       Space   _       Cmd     Opt     Macro4  Left    Down   Right  _
