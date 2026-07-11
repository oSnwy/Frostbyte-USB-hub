# Frostbyte-USB-hub


## What is this?
This is a simple USB hub, built using the Macondo tutorial. I put my own spin on things, using an SL2.1A and an external crystal, rather than relying on the internal crystal, making the PCB more reliable. Additionally, I wired capacitors in series rather than a single capacitor, minimizing the noise of the traces. I also designed a custom case to house the PCB.

<p align="center">
  <img src="https://github.com/oSnwy/Frostbyte-USB-hub/blob/main/Images/two%20halves%20w%20PCB.png" width="500"></p>
</p> 

| <img src="https://github.com/oSnwy/Frostbyte-USB-hub/blob/main/Images/two%20halves.png" width="333"> | <img src="https://github.com/oSnwy/Frostbyte-USB-hub/blob/main/Images/full%20set%20wo%20PCB.png" width="333"> | <img src="https://github.com/oSnwy/Frostbyte-USB-hub/blob/main/Images/full%20set%20w%20PCB.png" width="333"> |
| - | - | - |
### FEATURES:
- 1 Upstream USB-C port
- 2 Downstream USB-C ports
- 2 Downstream USB-A ports
- External 12mHz crystal for timing (More reliable than internal crystal from tutorial)
- Parallel 0.1uF and 10uF capacitors to further reduce noise, better than the tutorials singular 1uF capacitors

The case is designed to press fit into each other, using friction to keep the halves together. The PCB screwes into the bottom housing of the case through M2 screws.

ONSHAPE LINK: [OnShape](https://cad.onshape.com/documents/c9b467c6ac72e99f79eebd34/w/909402ed37444c79486434d0/e/d14026541bd022353ba53d64?renderMode=0&uiState=6a5196109ed6ccb7c50ef2e0)

## What if I want this?
If you want this exact USB hub, just download the [frostbyte-USB-Hub.zip](https://github.com/oSnwy/Frostbyte-USB-hub/blob/main/Gerber%20Files/frostbyte-USB-Hub.zip) from the Gerber Files folder, as well as the [bom.csv](https://github.com/oSnwy/Frostbyte-USB-hub/blob/main/JLCPCB%20files/bom.csv) and [positions.csv](https://github.com/oSnwy/Frostbyte-USB-hub/blob/main/JLCPCB%20files/positions.csv) from the JLCPCB files folder. Simply upload the files to [JCLPCB's Order Now](https://cart.jlcpcb.com/quote?spm=Jlcpcb.Homepage.1006&spm=Jlcpcb.Homepage.1006), and add these parts below to each footprint or use the links in the BOM below:
<p align="center">
  <img src="https://cdn.hackclub.com/019f4ce2-f427-7f11-b544-e7c3b1dbc62e/image.png" width="1000"></p>
</p> 
After that, all you need to do is add it to the cart!

If you'd like to make your own, all the resources I used are linked below! These are some helpful links that can get you started. Alternatively, you can follow my process documented in the journals below!

### PCB AND SCHEMATIC
| <img src="https://cdn.hackclub.com/019f48f9-906b-7fcd-889f-c5f5a08ec8b6/image.png" width="500"> | <img src="https://cdn.hackclub.com/019f49f3-bf44-7f6a-978a-f6750eb83ac8/image.png" width="500"> |
| - | - | 


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
Total cost, including assembly, comes to around $52.94 CAD from JLCPCB, or $37.32 USD. Attempting to order the PCB without assembly is not recommended due to the difficulty of soldering the crystal and capacitors.

## BOM for PCB
| PART | QTY | LINK |
| - | - |
| USB-C Receptacle | 3 | [LINK](https://jlcpcb.com/partdetail/Korean_HropartsElec-TYPE_C_31_M12/C165948) |
| USB-A Receptacle | 2 | [LINK](https://jlcpcb.com/partdetail/MOLEX-676432911/C293351) |
| 12mHz Crystal | 1 | [LINK](https://jlcpcb.com/partdetail/SST-S503212M20PF20PPMB/C7426819) |
| SL2.1A | 1 | [LINK](https://jlcpcb.com/partdetail/CoreChips-SL21A/C6798314) |
| 4.7R Resistor | 1 | [LINK](https://jlcpcb.com/parts/componentSearch?searchTxt=c23164) |
| 5.1K Resistor | 1 | [LINK](https://jlcpcb.com/parts/componentSearch?searchTxt=c23186) |
| 56K Resistor | 1 |  [LINK](https://jlcpcb.com/partdetail/23933-0603WAF5602T5E/C23206) |
| 10uF Capacitor | 5 | [LINK](https://jlcpcb.com/partdetail/16532-CL21A106KAYNNNE/C15850) |
| 4.7uF Capacitor | 3 | [LINK](https://jlcpcb.com/partdetail/2131-CL21A475KAQNNNE/C1779) |
| 0.1uF Capacitor | 7 | [LINK](https://jlcpcb.com/parts/componentSearch?searchTxt=c14663) |


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

## JOURNAL #4
LAPSE LINK: https://lapse.hackclub.com/timelapse/RwhSkVn_50UR
<p align="center">
  <img src="https://cdn.hackclub.com/019f4dd3-9121-7433-8df9-a8120ddd782b/Case%20Halves%20with%20PCB.png" width="1000"></p>
</p> 
I created the case for my USB hub. This was created in two parts that snap fit together, with M2 screw standoffs for the PCB to attach to. The PCB is sandwiched between the two parts of the case. This case was designed in TinkerCAD.

## JOURNAL #5
LAPSE LINK: https://lapse.hackclub.com/timelapse/sdaK7IJP7WCH
<p align="center">
  <img src="https://cdn.hackclub.com/019f4e94-6cd3-704e-b5a5-1db0c7831b94/two%20halves%20w%20PCB.png" width="1000"></p>
</p>
<p align="center">
  <img src="https://cdn.hackclub.com/019f4e99-56db-77dc-9de4-df1c46be5a46/two%20halves.png" width="1000"></p>
</p>
After checking the shipping requirements, it turns out that TinkerCad is not allowed because it doesn't provide the required source files. However, the time spent on TinkerCad was not wasted, as it became an extremely useful reference for 3d modelling on OnShape, as I could use the TinkerCad model for the dimensions, which ended up saving a lot of time. I probably should've read the shipping requirements, but I think using Tinkercad first still saved a little time.
