# esp32-s3-mini-1_CustomPCB_Altium
Integrating an ESP32-S3-Mini-1 module into a custom PCB design

ESP32-S3-MINI-1 module - (Xtensa® dual-core 32-bit LX7) featuring 2.4 GHz Wi-Fi and Bluetooth 5 (LE).

I designed a custom PCB, centered around ESP32-S3-MINI-1 module based on reference schematics and guidelines from official manufactoror and various diffrent datasheets.

Used 4-layer stackup to provide dedicated GND planes for EMI shielding. Completed full manual route of all components, applied clearances and most common rules in PCB desing (including "rooms" altium special feature).


Features and capabilities:
* Digital communication - dual-interface: USB-C to UART bridge and USB-C to esp32 (ESP32-S3's native USB OTG capability)
* Power management - stable 3.3V power trace using a LDO Regulator, implemented polygon pours for both power and GND.
* ESD protection circuits- TVS diode protection to protect the internal silicon from electrostatic.
* 24-pin headers (Header 1x24) providing access to the full suite of GPIOs, SPI, I2C, and PWM pins.
* On-board status LEDs and tactile boot and reset switches
* Boot/reset circuits using NPN transistors.
* Dual Power Input Protection - designed the power stage to safely handle power from the USB-C connector while maintaining thermal stability through the LDO regulator ???
* Differential Pair Implementation (Impedance Control) - controlled trace lengths and widths to maintain target impedance 90 ohms, in order to reject common-mode noise and reduce EMI radiation.


* **Check out the description for commits for more details on the work process.**


# Schematics

<p align="center">
  <img src="Outputs/schematics (1).png" width="70%">
  <img src="Outputs/schematics (4).png" width="70%">
  <img src="Outputs/schematics (2).png" width="70%">
  <img src="Outputs/schematics (3).png" width="70%">
</p>


# PCB

### Top Layer
<img src="\Outputs\pdf\layerTOP.png" >

### Bottom Layer
<img src="\Outputs\pdf\layerBottom.png" >

### Pwer and GND layers
<img src="\Outputs\pdf\layerGND.png" >
<img src="\Outputs\pdf\layerPower.png" >

### All layers together
<img src="\Outputs\entireThing (1).png" >
<img src="\Outputs\entireThing (2).png" >


### Top View
<img src="Outputs\topVIEW.png" >
<img src="Outputs\3d (2).png" >


### Bottom View 

<img src="Outputs\bottomVIEW.png" >
<img src="Outputs\3d (3).png" >



### Overall look
<p align="center">
<img src="\Outputs\3d (1).png" width="70%">
</p>



* **Check out the description for commits for more details on the work process.**

Altium 25.8.1