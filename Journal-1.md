# **Journal 1**

## *05/07/26 14:30 - 18:00*



## **The Plan + Schematic**



### **Theme**



I choose the name **"The Clanker"**



##### **Colors**



* Case: Sage green (#94B7AC)
* Keycaps: White
* Accent key (Esc or Enter): muted gray
* Knob: White or brushed aluminum
* RGB: Warm white by default with customizable effects



### **Plan**



#### **Features**



* Per-key RGB
* Rotary encoder
* 0.91" OLED
* USB-C (Pico)
* Silkscreen artwork
* Hot Swappable



#### **Keyboard Layout**



*5 row × 16 column matrix*



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



I started by placing the pico, and a single switch with diode



Once I had the keyboard layout figured out I copied and paste each switch and diode, making the matrix. Then I used net labels to connect to pico, GP0-GP18.



I added 4 mounting holes on the conners of whole matrix.



After this I wired the Oled and Encoder,
Encoder A - GP19

Encoder B - GP20

Encoder Switch - GP21



OLED SDA - GP26

OLED SCL - GP27



Then I Wired up the SK6812 MINI-E. I place 17 of them *(I'll Copy the rest in the PCB)* I connected the first led to GP22 and then put the rest in series.

I connect them all to 5v and gnd and put a 100µF capacitor on those rails.

I also put a 330Ω Resistor on the first led to the Pico.



Lastly I Annotated the schematic

