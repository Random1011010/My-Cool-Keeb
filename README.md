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



## 📋 Bill of Materials (BOM)

| Part Description | Qty | Link | Unit Cost (USD) | Total Cost (USD) |
| :--- | :---: | :--- | :---: | :---: |
| Orpheus Pico Microcontroller | 1 | [Hack Club Orpheus Pico](https://github.com/hackclub/orpheus-pico) | $0.00 | $0.00 |
| Outemu Silent White Linear Switches (90 pcs) | 90 | [AliExpress](https://www.aliexpress.com/item/1005002378701948.html) | $0.27 | $23.90 |
| 132-Key White Blank MOA Profile PBT Keycaps | 1 | [AliExpress](https://www.aliexpress.com/) | $20.96 | $20.96 |
| 1N4148 Diodes (100-pack for switch matrix & encoders) | 100 | [AliExpress](https://www.aliexpress.com/item/1005002339916163.html) | $0.016 | $1.64 |
| EC11 20mm Rotary Encoders (2-pack) | 1 | [AliExpress](https://www.aliexpress.com/) | $3.50 | $3.50 |
| M3 x 20mm Stainless Steel Screws (100-pack) | 100 | [AliExpress](https://www.aliexpress.com/) | $0.052 | $5.22 |
| HANGLIFE M3 Brass Heat-Set Inserts (100-pack) | 100 | [Amazon Canada](https://www.amazon.ca/) | $0.057 | $5.66 |
| Chosfox V3 Plate Mount Stabilizers Kit | 1 | [AliExpress](https://www.aliexpress.com/item/1005007299976098.html) | $8.57 | $8.57 |
| Custom PCB Fabrication & Delivery (5 pcs total) | 1 | [JLCPCB](https://jlcpcb.com/) | $58.85 | $58.85 |
| **Total** | | | | **~$128.30 USD** |
