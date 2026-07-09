# Frostbyte-USB-hub


## JOURNAL #1
 July 9th 2026: 2:24 hours
LAPSE LINK: https://lapse.hackclub.com/timelapse/4U5zvK8HuuRQ

<p align="center">
  <img src="https://cdn.hackclub.com/019f48f9-906b-7fcd-889f-c5f5a08ec8b6/image.png" width="1000"></p>
</p>

I created the schematic for my USB hub, using 1 USB-C port for upstream, and 2 USB-C ports and 2 USB-A ports for downstream, loosely following the Macondo tutorial and other sources. On top of the tutorial, I added a 12 mHz crystal, tweaked the capacitor and resistor values, and added capacitors in parallel for reliability. In order to figure out the resistor values, I used the original data sheet example, as well as other examples of USB hubs also using the SL2.1A, as the Macondo tutorial used a similar but different SL2.1S. Although they could be wired the same, I wanted to improve upon the tutorial, rather than blindly following it, requiring me to understand each part of the schematic.

<p align="center">
  <img src="https://cdn.hackclub.com/019f48fb-5233-7a57-bbd4-57290bc48704/image.png" width="1000"></p>
</p> 

I also assigned the footprints for the schematic, allowing me to move on to the next step of making the PCB. These parts were found through examples online, as well as the most common parts used.

RESOURCES USED: 
| Use | Website Link |
| - | - |
| Crystal Example | https://github.com/xunker/simple_sl2.1a_usb_hub |
| Crystal Example 2 | https://oshwlab.com/oshwlab/USB-concentrator-Based-on-SL2.1A |
| Crystal Example 3 | https://github.com/Hugoyhu/SL2.1A-Type-C-Hub |
| Data Sheet | https://www.lcsc.com/datasheet/C6798314.pdf?spm=wm.sxq.inf.ggs___wm.fly.bg.1.xh&lcsc_vid=EQVWVVVTFAVWAwUDQVkNBFdSRQBZBFJeR1UIBFYHTgUxVlNeRFdcUFFURlRdXjsOAxUeFF5JWBYZEEoKFBINSQcJGk4eFQsCAgIaSgADAwAHC0slRVdWU1BVRE8GEwkK |
| Footprint and Symbol Download | https://www.snapeda.com/parts/SL2.1A/CoreChips%20ShenZhen%20CO.,Ltd/view-part/?company=Maple&amp;welcome=home |
