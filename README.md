# The Clanker

# 

# **The Clanker** is a fully custom mechanical keyboard designed from scratch using **KiCad** for the electronics and **Fusion 360** for the case. The goal of this project was to design every part of the keyboard myself, from the schematic and PCB layout to the enclosure and firmware.

The keyboard features a compact 68-key layout, per-key RGB lighting, a rotary encoder, and a 0.91" OLED display, all powered by a Raspberry Pi Pico.


## Features

* 68-key custom layout

* Raspberry Pi Pico (USB-C)

* MX switches

* Per-key SK6812 MINI-E RGB lighting

* Rotary encoder

* 0.91" I²C OLED display

* Custom 3D-printable case

* Designed entirely from scratch

## Design Process
The project began by creating the keyboard layout and designing the schematic in KiCad. After assigning footprints, the PCB was laid out and routed, including the switch matrix, RGB LEDs, OLED display, rotary encoder, and power circuitry.
Once the PCB was complete, it was exported into Fusion 360 where the enclosure was designed around it. The case was built specifically for 3D printing and split into two halves so it could fit on a smaller print bed while remaining rigid once assembled.

## BOM

| Item                   | Qty | Notes                  |   $   | URL |
| ---------------------- | --: | ---------------------- | :--:  | ---- |
| Raspberry Pi Pico      |   1 | RP2040 microcontroller | 9.23  | [link](https://www.aliexpress.com/item/1005011871301955.html?pdp_ext_f=%7B"order"%3A"19"%2C"eval"%3A"1"%2C"fromPage"%3A"search"%7D) |
| MX Mechanical Switches |  68 | Cherry MX compatible   | 30.22 | [link](https://www.aliexpress.com/item/1005008998414457.html?pdp_ext_f=%7B"order"%3A"322"%2C"eval"%3A"1"%2C"fromPage"%3A"search"%7D) |
| PCB Mount Stabilizers  |   4 | For larger keys        | 11.23 | [link](https://www.aliexpress.com/item/1005001686299616.html?pdp_ext_f=%7B"order"%3A"267"%2C"eval"%3A"1"%2C"fromPage"%3A"search"%7D) |
| LEDs                   |  68 | One per switch         | 8.68 | [link](https://www.aliexpress.com/item/1005006727416963.html?pdp_ext_f=%7B"order"%3A"59"%2C"spu_best_type"%3A"price"%2C"eval"%3A"1"%2C"fromPage"%3A"search"%7D) |
| Keycap Set             |   1 | 68-key compatible      | 24.17 | [link](https://www.aliexpress.com/item/1005007252695395.html?pdp_ext_f=%7B"order"%3A"68"%2C"eval"%3A"1"%2C"fromPage"%3A"search"%7D) |
| Rotary Encoder         |   1 | EC11                   | 9.84 | [link](https://www.aliexpress.com/item/1005011653314162.html?pdp_ext_f=%7B"order"%3A"8"%2C"eval"%3A"1"%2C"fromPage"%3A"search"%7D) |
| Encoder Knob           |   1 | Fits encoder shaft     | 1.76 | [link](https://www.aliexpress.com/item/1005008291630040.html?aem_p4p_detail=20260710071720613074789560480005766622&pdp_ext_f=%7B"order"%3A"224"%2C"spu_best_type"%3A"price"%2C"eval"%3A"1"%2C"fromPage"%3A"search"%7D&search_p4p_id=20260710071720613074789560480005766622_6) |
| OLED Display           |   1 | .91" I2C (SSD1306)   | 1.44 | [link](https://www.aliexpress.com/item/1005008997559133.html?pdp_ext_f=%7B"order"%3A"2411"%2C"eval"%3A"1"%2C"fromPage"%3A"search"%7D) |
| PCB                    |   1 | Custom keyboard PCB    | 61.97 | [link](https://github.com/user-attachments/assets/7c825ecb-10aa-4597-84ef-201b4d64e1a1) |
|  |  |  *Shipping* |  *5.71* | |
|  |  |  *Dutes* |  *8.27* |  |
|  |  | **Total** |  **109.56** | |


## Gallery



|                   PCB                  |                   Schematic                  |                CAD Model               |
| :------------------------------------: | :------------------------------------------: | :------------------------------------: |
| <img width="1463" height="619" alt="Screenshot 2026-07-08 183934" src="https://github.com/user-attachments/assets/52bf7a74-9dcb-4d7a-b39d-324447c115f4" /> | <img width="1848" height="810" alt="Screenshot 2026-07-08 184029" src="https://github.com/user-attachments/assets/62c53c45-1019-4890-bde3-c2f47449ec9b" /> | <img width="1556" height="912" alt="Screenshot 2026-07-08 183543" src="https://github.com/user-attachments/assets/2e6c6dee-cce2-4253-ba4b-a905232df095" /> |



