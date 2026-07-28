# My-Cool-Keeb
# Name: Morning Star

**Morning Star** is a custom 81-key mechanical keyboard powered by the **Hack Club Orpheus Pico** (RP2040). Built with dual rotary encoders, ultra-quiet linear switches, and a custom 2-layer PCB inside a 3D-printed enclosure, it delivers a high-functionality, low-noise typing experience.

<img width="878" height="403" alt="Screenshot 2026-07-28 at 3 13 28 PM" src="https://github.com/user-attachments/assets/95b141b5-8424-4be6-bc75-8c00a310a39d" />

---

## 🛠️ Project Writeup

### What I Built
Morning Star is a custom-designed, 81-key mechanical keyboard featuring a dedicated function row, arrow cluster, and dual EC11 rotary encoders. 

* **Microcontroller**: Powered by the Hack Club Orpheus Pico (RP2040).
* **Sound Profile**: Engineered for silent operation using Outemu Silent White linear switches, blank MOA profile PBT keycaps, and pre-clipped Chosfox V3 plate-mount stabilizers.
* **PCB & Hardware**: Custom 2-layer PCB designed, housed in a 3D-printed enclosure held together with M3 brass heat-set inserts and stainless steel hex socket screws.

---

### Why I Built It
Standard off-the-shelf mechanical keyboards are often either too noisy for shared environments or lack the physical control density needed for media editing, live sound workflows, and rapid navigation. 

I wanted to design a custom board from scratch that solved these problems:
1. **Dual Encoder Control**: Placing two tactile knobs directly on the layout gives instant physical control over volume, timeline scrubbing, and macro adjustments without leaving the home row.
2. **Silent Treatment**: By choosing silent white linear switches and plate-mounted stabilizers with pre-clipped stems, I wanted to eliminate rattle and any noise (I study at night so I would get in trouble if it was loud).

---

### What I Learned
Building Morning Star involved learning hardware production, PCB fabrication constraints, and firmware matrix logic:

* **PCB Manufacturing & Cost Optimization**: I learned how small design decisions directly impact manufacturing price. By selecting "Tented" via covering, I eliminated extra processing surcharges on JLCPCB while keeping standard matrix routing intact.
* **Hardware Sourcing & Budgeting**: Balancing component lead times and shipping fees taught me how to structure a realistic Bill of Materials across multiple suppliers (AliExpress, Amazon, JLCPCB) while staying strictly within budget limits.
* **Mechanical Design & Fasteners**: I learned why direct-threading screws into 3D-printed plastic leads to stripped threads over time, and how using a soldering iron to melt brass heat-set inserts into internal bosses provides strong, long-lasting metal threads for continuous teardowns.
* **Matrix Logic & Firmware**: I gained experience configuring diode-isolated key matrices (1N4148 diodes) to ensure full N-Key Rollover (NKRO) without ghosting, as well as mapping quadrature encoder signals to GPIO pins on the RP2040.

---

## 📋 Bill of Materials (BOM)

| Part Description | Qty | Unit Cost (USD) | Total Cost (USD) | Source / Link |
| :--- | :---: | :---: | :---: | :--- |
| **Orpheus Pico Microcontroller** | 1 | $0.00 | $0.00 | [Hack Club GitHub](https://github.com/hackclub/orpheus-pico) |
| **Outemu Silent White Linear Switches** (90 pcs) | 90 | $0.27 | $23.90 | [AliExpress](https://www.aliexpress.com/item/1005002378701948.html) |
| **132-Key White Blank MOA Profile Keycaps** | 1 | $20.96 | $20.96 | [AliExpress](https://www.aliexpress.com/) |
| **1N4148 Signal Diodes** (100-pack) | 100 | $0.016 | $1.64 | [AliExpress](https://www.aliexpress.com/item/1005002339916163.html) |
| **EC11 20mm Rotary Encoders** (2-pack) | 1 | $3.50 | $3.50 | [AliExpress](https://www.aliexpress.com/) |
| **M3 x 20mm Stainless Steel Screws** (100-pack) | 100 | $0.052 | $5.22 | [AliExpress](https://www.aliexpress.com/) |
| **HANGLIFE M3 Brass Heat-Set Inserts** (100-pack) | 100 | $0.057 | $5.66 | [Amazon Canada](https://www.amazon.ca/) |
| **Chosfox V3 Plate Mount Stabilizers Kit** | 1 | $8.57 | $8.57 | [AliExpress](https://www.aliexpress.com/item/1005007299976098.html) |
| **Custom 2-Layer PCB Fabrication** (5 pcs total) | 1 | $58.85 | $58.85 | [JLCPCB](https://jlcpcb.com/) |
| **Total Estimated Cost** | | | **~$128.30 USD** | |

---

## 🛠️ Hardware Specifications

* **MCU**: Hack Club Orpheus Pico (RP2040)
* **Matrix Architecture**
* **Encoders**: 2x EC11 5-pin encoders connected to dedicated GPIO channels.
* **Enclosure Fasteners**: M3 x D5 x L4 mm brass heat-set inserts with M3 x 20mm.
* **Stabilizers**: Chosfox V3 plate-mount stabilizers for keycaps ≥ 2u.
