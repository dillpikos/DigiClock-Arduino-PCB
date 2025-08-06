# Digital Clock PCB Created With KiCAD 9

A custom designed digital clock PCB that integrates an Ardunio Nano, the SSD1306 OLED Display, and the DS3231 RTC Module to display the current time and day of the year.
</br>
All components were selected for compatibility and the PCB includes custom made symbols and footprints for the RTC module and the OLED display along with labeling on the silkscreen of the PCB for clairity.
</br>
</br>
This system includes an onboard battery health check system which detects if the backpack battery on the RTC module is either dead or was removed while the device was unplugged (meaning the time is wrong and needs to be reset) A pop up makes sure the user knows of this and it lasts for 10 seconds upon the start of the device
</br>
</br>
This board is meant to operate at 3.3V, uses I2C to communicate to all components and has mounting holes in each corner for M2 screws
</br>
*created by Bryan Diaz | Focus: Embedded Systems, Hardware, and PCB Design*

# Technologies and Components

## Hardware Related:
+ Arduino Nano
+ DS3231 Real Time Clock Module
+ SSD1306 0.96' OLED Display
+ Custom 2 layer PCB (designed in KiCAD)
+ Soldering of through hole components

## Software Related:
+ Arduino IDE
+ C++ (custom functions for retrieving time and date, battery health check system, drawing UI upon the start of the device)
+ Various Libraries for Components
  + Adafruit GFX
  + Adafruit_SSD1306
  + RTClib
+ KiCAD 9 (Used for schematic design and layout, along with custom symbols and footprints for modules)
+ Gerber File generation for manufacturing (manufactured using PCBWay)


## Custom Footprints
Footprints were created for the PCB based on the exact physical measurments of the components in mm for accurate pad and pin allignments (2.54 mm spacing between pads)
- DS3231 RTC Module: 22mm x 38.5mm (W x L) 
- SSD1306 Display : 28mm x 28mm (W x L)


# System Preview
<img src = "https://github.com/user-attachments/assets/936329aa-14d0-4de2-b1b4-fcba4635303b" width = "550" height = "550"/> 
<img src = "https://github.com/user-attachments/assets/b9eb7865-8bd0-446e-9074-16d83d67c04f" width = "550" height = "550"/> 
<img src = "https://github.com/user-attachments/assets/255c8900-673d-4ea4-8817-17b267f5f92a" width = "550" height = "550"/> 

# Battery Health Check System Preview
<img src = "https://github.com/user-attachments/assets/2c916758-e5f6-4924-934b-60bfe770b088" width = "550" height = "550"/> 

