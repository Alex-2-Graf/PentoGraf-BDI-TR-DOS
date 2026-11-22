# PentoGraf-BDI-TR-DOS  
  
> [English](README.en.md) | [Русский](README.md)
>
> 
## Beta Disk Interface (TR-DOS) controller for PentoGraf. Supports up to 4 drives, onboard +12V DC-DC converter, Reset to Bank 0, and 2 PLL versions (FDC9216 / KR556RT4A).
  
---
  
This project is an implementation of the Beta Disk Interface (BDI) for PentoGraf, which was originally omitted from the mainboard.

* **Key Features:** Support for up to 4 floppy drives (A, B, C, D), proper Reset to ROM Bank 0, onboard +12V DC-DC converter, LED indicators for power (+5V, +12V) and disk activity, as well as compatibility with KR1818VG93 (WD1793) emulators.
  
---
  
## PLL Board Versions:  
  
Based on the FDC9216B chip (stable digital data separator requiring no adjustment):  
  
[iBOM](Export/BDI%20PentoGraf%20(FDC9216B).html) [Schematic](Export/BDI%20PentoGraf%20(FDC9216B).pdf) [Gerber](Gerber/BDI%20PentoGraf%20(FDC9216B)_Gerber.zip)  
  
![](Images/BDI%20PentoGraf%20(FDC9216B)_PCB.png)  
  
![](Images/BDI%20PentoGraf%20(FDC9216B)_BDI.png)  
  
![](Images/BDI%20PentoGraf%20(FDC9216B).jpg)  
  
---
  
Classic version based on the KR556RT4A (82S129) PROM for reliable reading of worn or "difficult" floppy disks:  
  
[iBOM](Export/BDI%20PentoGraf%20(PT4A).html) [Schematic](Export/BDI%20PentoGraf%20(PT4A).pdf) [Gerber](Gerber/BDI%20PentoGraf%20(PT4A)_Gerber.zip) [RT4](ROM/556RT4.bin)  
  
![](Images/BDI%20PentoGraf%20(PT4A)_PCB.png)  
  
![](Images/BDI%20PentoGraf%20(PT4A)_BDI.png)  
  
![](Images/BDI%20PentoGraf%20(PT4A).jpg)  
  
---
  
## Unification  
  
Both PCB versions share identical outer dimensions and mounting hole locations.  
This allows you to easily swap one controller revision for another within the same enclosure.  
  
## Technical Notes:  
  
The controllers are designed for seamless (Plug-and-Play) connection to my mainboard revision:
  
* [PentoGraf-Pentagon-1024k](https://github.com)

However, they can also be used with other ZX Spectrum clones via the NEMO-bus.
  
A [KR1818VG93 (WD1793) emulator](https://github.com) can be used instead of the original FDC chip.
  
When using known-good components and quality soldering, no calibration or adjustment is required.  
