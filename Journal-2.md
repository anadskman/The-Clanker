# **Journal-2**

## *05/07/26 19:00 - 22:00*

## *06/07/26 12:00 - 16:00*

## *Total:* \~**7**hrs



## **Footprints + PCB**



#### **Footprints**



* Pico - RaspberryPi\_Pico\_Common\_THT
* Diodes - Diode\_THT:D\_DO-35\_SOD27\_P7.62mm\_Horizontal
* Switches - PCM\_marbastlib-mx:SW\_MX\_1u
* Stabilizers - PCM\_marbastlib-mx:STAB\_MX\_P\_2.25u
* Mounting Holes - MountingHole\_3.2mm\_M3
* LEDs - LED\_SK6812MINI-E
* Rotary - PCM\_marbastlib-various:ROT\_Alps\_EC11E-Switch
* OLED - Display:ER\_OLEDM0.91\_1x-I2C
* Resistor - Resistor\_THT:R\_Axial\_DIN0207\_L6.3mm\_D2.5mm\_P7.62mm\_Horizontal
* Cap - Capacitor\_THT:CP\_Radial\_D5.0mm\_P2.50mm



### **PCB**

I after I assigned the footprints I set my scale to 19.05mm(1u) and tried placing all the keys and stabs.
however for some reason it didn't look right and wasn't lining up right.

I updated Matrix as it wasn't quite how I wanted, but this turned out to be good as I noticed the cols were wired into the rows instead of across.

I also updated the stabs footprints so space is 6.25u, and then 2x 2.25u and a 2u.
I also added grid for .25u, .5u, and .75u and this made it a lot easier to layout they keys. I even added .125u.

I indent row1 by .25u, row2 by .5u, and row3 by .75u.



After all the keys and stabs were placed I test where I want the pico.

I originally had it on the right but since I wanted the rotary and oled on the top left corner I ended up moving it over there.



Then I placed all the diodes out which took for ever, along with the Leds but I put the Leds in B.Cu by pressing `f` and placed them just under the keys.

But after thinking about it I moved each led back to F.Cu and put them in-between the keys

I moved the pico back the right side as my pc sits on the right.

I then slowly routed everything, the leds I had to rotate them all 180 deg ivdivulialy so the in out pins align.
But for some reason every so led was in the wrong place, for example 10, 12, 11, instead of 10, 11, 12. which messes with the routed so I tried fixing it.

But I think the problem was in the schematic I only made 17 leds and in the pcb just copied them over, so Instead I made all 68 led in the schematic and slowly put the new ones in place.



Once the leds were wired up to resistor and pico I did the oled a encoder signal pins.



Finally all the GPIO pins are done.

Now Gnd, 3.3v and 5v.



For Gnd im just doing a gnd fill

5v for I used .7mm tracks as there is a lot of stuff on them



I ran DRC but its giving me 330+ errors about thermal, unconnections, ect.

so I spent maybe 30mins atleast fixing, and debugging all of it.

I solved a fair bit of it and the rest are not to worry about(Hopefully)



**Row0(*Numbers*)**

| Key       | Row | Col |

| --------- | --- | --- |

| Esc       | R0  | C0  |

| 1         | R0  | C1  |

| 2         | R0  | C2  |

| 3         | R0  | C3  |

| 4         | R0  | C4  |

| 5         | R0  | C5  |

| 6         | R0  | C6  |

| 7         | R0  | C7  |

| 8         | R0  | C8  |

| 9         | R0  | C9  |

| 0         | R0  | C10 |

| -         | R0  | C11 |

| =         | R0  | C12 |

| Backspace | R0  | C13 |

| Del       | R0  | C14 |



**Row1(*Q*)**

| Key | Row | Col |

| --- | --- | --- |

| Tab | R1  | C0  |

| Q   | R1  | C1  |

| W   | R1  | C2  |

| E   | R1  | C3  |

| R   | R1  | C4  |

| T   | R1  | C5  |

| Y   | R1  | C6  |

| U   | R1  | C7  |

| I   | R1  | C8  |

| O   | R1  | C9  |

| P   | R1  | C10 |

| \[   | R1  | C11 |

| ]   | R1  | C12 |

| \\   | R1  | C13 |

| `   | R1  | C14 |





**Row2(*Home*)**

| Key   | Row | Col |

| ----- | --- | --- |

| Caps  | R2  | C0  |

| A     | R2  | C1  |

| S     | R2  | C2  |

| D     | R2  | C3  |

| F     | R2  | C4  |

| G     | R2  | C5  |

| H     | R2  | C6  |

| J     | R2  | C7  |

| K     | R2  | C8  |

| L     | R2  | C9  |

| ;     | R2  | C10 |

| '     | R2  | C11 |

| Enter | R2  | C12 |

| pgup  | R2  | C14 |





**Row3(*Shift*)**

| Key   | Row | Col |

| ----- | --- | --- |

| Shift | R3  | C0  |

| Z     | R3  | C1  |

| X     | R3  | C2  |

| C     | R3  | C3  |

| V     | R3  | C4  |

| B     | R3  | C5  |

| N     | R3  | C6  |

| M     | R3  | C7  |

| ,     | R3  | C8  |

| .     | R3  | C9  |

| /     | R3  | C10 |

| Shift | R3  | C11 |

| ↑     | R3  | C13 |

| pgdn  | R3  | C14 |





**Row4(*Bottom*)**

| Key    | Row | Col |

| -----  | --- | --- |

| Ctrl   | R4  | C0  |

| Win    | R4  | C1  |

| Alt    | R4  | C2  |

| Space  | R4  | C3  |

| Alt gr | R4  | C9  |

| Fn     | R4  | C10 |

| Ctrl   | R4  | C11 |

| ←      | R4  | C12 |

| ↓      | R4  | C13 |

| →      | R4  | C14 |







| Offset |       Distance |

| ------ | -------------: |

| 0.25u  |  \*\*4.7625 mm\*\* |

| 0.5u   |   \*\*9.525 mm\*\* |

| 0.75u  | \*\*14.2875 mm\*\* |

| 1u     |   \*\*19.05 mm\*\* |



look through chat for what progress - basically everything pcb, redesign as it wasn't working, added keys to schematic



If your footprint only has 3 pads → WRONG version.



Orientation rule:



All LEDs must face the same direction OR follow chain direction.



We’ll handle rotation later in PCB stage.

