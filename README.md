# Frostbyte-USB-hub


## What is this?
This is a simple USB hub, built using the Macondo tutorial. I put my own spin on things, using a SL2.1A and an external crystal, rather than relying on the internal crystal. This makes the PCB more reliable. Additionally, I wired capacitors in series rather than a single capacitor, minimizing the noise of the traces.

### FEATURES:
- 1 Upstream USB-C port
- 2 Downstream USB-C ports
- 2 Downstream USB-A ports

## What if I want this?
If you want this exact USB hub, just download the [frostbyte-USB-Hub.zip](Gerber Files/frostbyte-USB-Hub.zip) from the Gerber Files folder, as well as the [bom.csv](JLCPCB files/bom.csv) and [positions.csv](JLCPCB files/positions.csv) from the JLCPCB files folder. Simply upload the files to [JCLPCB's Order Now](https://cart.jlcpcb.com/quote?spm=Jlcpcb.Homepage.1006&spm=Jlcpcb.Homepage.1006), and add these parts below to each footprint:
<p align="center">
  <img src="https://cdn.hackclub.com/019f4ce2-f427-7f11-b544-e7c3b1dbc62e/image.png" width="1000"></p>
</p> 
After that, all you need to do it add it to cart!

If you'd like to make your own, all the resources I used are linked below! These are some helpful links that can get you started.


### RESOURCES USED: 
| Use | Website Link |
| - | - |
| Macondo Tutorial | [Macondo](https://macondo.hackclub.com/docs/usb-hub) |
| Crystal Example | [Github](https://github.com/xunker/simple_sl2.1a_usb_hub) |
| Crystal Example 2 | [Oshwlab](https://oshwlab.com/oshwlab/USB-concentrator-Based-on-SL2.1A) |
| Crystal Example 3 | [Github](https://github.com/Hugoyhu/SL2.1A-Type-C-Hub) |
| Data Sheet | [LCSC](https://www.lcsc.com/datasheet/C6798314.pdf?spm=wm.sxq.inf.ggs___wm.fly.bg.1.xh&lcsc_vid=EQVWVVVTFAVWAwUDQVkNBFdSRQBZBFJeR1UIBFYHTgUxVlNeRFdcUFFURlRdXjsOAxUeFF5JWBYZEEoKFBINSQcJGk4eFQsCAgIaSgADAwAHC0slRVdWU1BVRE8GEwkK) |
| Footprint and Symbol Download | [SnapEDA](https://www.snapeda.com/parts/SL2.1A/CoreChips%20ShenZhen%20CO.,Ltd/view-part/?company=Maple&amp;welcome=home) |

## TOTAL COST
Total cost including assembly comes to around $52.94 CAD from JLCPCB. Attempting to order the PCB without assembly is not recommended due to the difficulty of soldering the crystal and capacitors.

## BOM for PCB
| PART | QTY |
| - | - |
| USB-C Receptacle | 3 |
| USB-A Receptacle | 2 |
| 12mHz Crystal | 1 |
| SL2.1A | 1 |
| 4.7R Resistor | 1 |
| 5.1K Resistor | 1 |
| 56K Resistor | 1 | 
| 10uF Capacitor | 5 |
| 4.7uF Capacitor | 3 |
| 0.1uF Capacitor | 7 |


## JOURNALS

### JOURNAL #1
- July 9th 2026: 2:24 hours
LAPSE LINK: https://lapse.hackclub.com/timelapse/4U5zvK8HuuRQ

<p align="center">
  <img src="https://cdn.hackclub.com/019f48f9-906b-7fcd-889f-c5f5a08ec8b6/image.png" width="1000"></p>
</p>

I created the schematic for my USB hub, using 1 USB-C port for upstream, and 2 USB-C ports and 2 USB-A ports for downstream, loosely following the Macondo tutorial and other sources. On top of the tutorial, I added a 12 mHz crystal, tweaked the capacitor and resistor values, and added capacitors in parallel for reliability. In order to figure out the resistor values, I used the original data sheet example, as well as other examples of USB hubs also using the SL2.1A, as the Macondo tutorial used a similar but different SL2.1S. Although they could be wired the same, I wanted to improve upon the tutorial, rather than blindly following it, requiring me to understand each part of the schematic.

<p align="center">
  <img src="https://cdn.hackclub.com/019f48fb-5233-7a57-bbd4-57290bc48704/image.png" width="1000"></p>
</p> 

I also assigned the footprints for the schematic, allowing me to move on to the next step of making the PCB. These parts were found through examples online, as well as the most common parts used.



### JOURNAL #2
- July 9th 2026: 3:10 hours
LAPSE LINK: https://lapse.hackclub.com/timelapse/BneAj1DRkeYR
I started on the creation of the PCB. Despite minor setbacks, such as accidentally assigning the sl2.1a footprint to the capacitor, accidentally using a 4-pin crystal instead of a 2-pin crystal, forgot 0.1uF needs to be close to the pins to make it more effective, putting the usb a ports backwards, needing to put the d+ and d- traces closer and having to move traces away from 12mHz crystal, majority of the pcb was eventually wired. I had to wire it multiple times to make it both neat and efficient.

<p align="center">
  <img src="https://cdn.hackclub.com/019f49f3-bf44-7f6a-978a-f6750eb83ac8/image.png" width="1000"></p>
</p>
I also created a BOM and CPL for the pieces and positions of the PCB. However, the 12mHz crystals in the JLCPCB stock didn't match the footprint and needs of my crystal. The next step is to change the footprint of the 12mHz crystal in order to match a crystal in stock at JLCPCB, as soldering one can be extremely challenging and requires specific tools.
<p align="center">
  <img src="https://cdn.hackclub.com/019f49fc-2631-7839-aa46-4ebdf9e29b62/image.png" width="1000"></p>
</p>


### JOURNAL #3
LAPSE LINK: https://lapse.hackclub.com/timelapse/NV_NpuBsBBrh

UPDATED PCB:
<p align="center">
  <img src="https://cdn.hackclub.com/019f4cec-712f-783f-84b2-7799c0a6018f/image.png" width="1000"></p>
</p> 
It's done! Despite using the wrong 12 mHz Crystal three times, I finally managed to get the correct footprint and match a correct part onto the board in JLCPCB. I had to edit the PCB a few times and reupload the Gerber files in order for it to work, but it worked out in the end.

Empty PCB:
<p align="center">
  <img src="https://cdn.hackclub.com/019f4ce2-cec6-7648-86d2-b2f62d7d18d1/image.png" width="1000"></p>
</p> 
BOM parts:
<p align="center">
  <img src="https://cdn.hackclub.com/019f4ce2-f427-7f11-b544-e7c3b1dbc62e/image.png" width="1000"></p>
</p> 
3d Render:
<p align="center">
  <img src="https://cdn.hackclub.com/019f4ce3-c4dd-7c74-806f-ed8ec1874e41/image.png" width="1000"></p>
</p> 
Final Price:
<p align="center">
  <img src="https://cdn.hackclub.com/019f4cec-349a-7e75-bf8f-604507dccd9d/image.png" width="1000"></p>
</p> 
