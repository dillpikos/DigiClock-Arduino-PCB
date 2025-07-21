# Digital Clock PCB Created With KiCad 9

A custom designed digital clock PCB that integrates an Ardunio Nano, the SSD1306 OLED Display, and the DS3231 RTC Module to display the current time and day of the year.
</br>
</br>
All components were selected for compatibility and the PCB includes custom made symbols and footprints for the RTC module and the OLED display along with labeling on the silkscreen of the PCB for clairity.
</br>
</br>
This system includes an onboard battery health check system which detects if the backpack battery on the RTC module is either dead or was removed while the device was unplugged (meaning the time is wrong and needs to be reset) A pop up makes sure the user knows of this and it lasts for 10 seconds upon the start of the device
</br>
</br>
This board is meant to operate at 3.3V and uses I2C to communicate to all components
</br>
*created by Bryan Diaz | Focus: Embedded Systems, Hardware, and PCB Design*

# Technologies and Componenets

## Hardware Related:
+ Arduino Nano
+ DS3231 Real Time Clock Module
+ SSD1306 0.96' OLED Display
+ Custom 2 layer PCB (designed in KiCad)
+ Soldering of through hole components

## Software Related:
+ Arduino IDE
+ C++ (custom functions for retrieving time and date, bettery health check system, drawing UI upon the start of the device)
+ Various Libraries for Components
  + Adafruit GFX
  + Adafruit_SSD1306
  + RTClib
+ KiCad9 (Used for schematic design and layout, along with custom symbols and footprints for modules)



## Custom Footprints
Footprints were create for the PCB based on the exact physical measurments of the components in MM

