# buddipole-rotator

Inspired by [the rotator made by KI6AWR and HB9MTN](https://qsl.net/hb9mtn/BPMW/MW_Rotor.html), this rotator adds some additional features and makes some design changes. All of the rotator intelligence is located in the rotator at the mast and exposes an RS485 connection with the [Idiom Press Rotor-EZ Rotator Control Protocol](https://www.hamsupply.com/wp-content/uploads/2015/11/Rotor-EZ-Protocol.pdf).

I've split this into a few independent designs and parts

- Rotator
- Controller
- Wireless Module

## Rotator 

### Features
- Utilizes [Idiom Press Rotor-EZ Rotator Control Protocol](https://www.hamsupply.com/wp-content/uploads/2015/11/Rotor-EZ-Protocol.pdf) over Full Duplex RS-485
- Trinamic TMC2130 Stepper driver can intelligently adjust power output to the stepper based on load to prevent lost steps, maximize motor torque, reduce power consumption, and heat output
- Can operate off of wide voltage range (max input voltage 21V)
- 1° rotation increments
  
### Design
- Arduino Code - Link to Arduino Source Code
- Schematic - Link to Schematic
- Board - Link to board
- STL files - Link to STL files

### Parts
- Stepper [Nema 17 Bipolar 1.5A 42Ncm 42x42x38mm 1.8deg](https://www.amazon.com/STEPPERONLINE-Stepper-Bipolar-42x42x38mm-Connector/dp/B0B38GX54H)
- Stepper Driver - [SilentStepStick w/TMC2130](https://learn.watterott.com/silentstepstick/)
- Stepper Driver Protection - [SilentStepStick Protector](https://learn.watterott.com/silentstepstick/protector/)
- Microcontroller - [Ardunio Nano Every](https://store-usa.arduino.cc/products/arduino-nano-every)
- Level Shifter (RS485 to TTL) - MAX488EPA+ - [Digikey](https://www.digikey.com/en/products/detail/analog-devices-inc-maxim-integrated/MAX488EPA/1495109?s=N4IgTCBcDaILIEEAaAWAHGgogBQQagAIQBdAXyA) | [Mouser](https://www.mouser.com/ProductDetail/Analog-Devices-Maxim-Integrated/MAX488EPA%2b?qs=1THa7WoU59G6dxfe6rTcAA%3D%3D)
- Connectors
  - Power - Anderson Powerpole 15/45
  - Communication - 5-pin M12 A-Code Circular Connectors [DigiKey](https://www.digikey.com/en/products/detail/conec/43-01199/2793477?s=N4IgTCBcDaIAQBYDMBaADARgwTmyAugL5A)/[Mouser](https://www.mouser.com/ProductDetail/Amphenol-CONEC/43-01199?qs=BLWaPj7617f34EH%2FcnQWlA%3D%3D)

## Controller

### Features
- Clear visual indicators of antenna status and any pending moves to be made
- Easy to use buttons
  - Cardinal direction buttons for quick access
  - CW/CCW buttons for finer adjustment
- LCD screen for adjusting settings / detailed readout of status
- Utilizes [Idiom Press Rotor-EZ Rotator Control Protocol](https://www.hamsupply.com/wp-content/uploads/2015/11/Rotor-EZ-Protocol.pdf) over Full Duplex RS-485 via 5-pin 16mm aviation connector

### Design
- Arduino Code - Link to Arduino Source Code
- Schematic - Link to Schematic
- Board - Link to board
- STL files - Link to STL files

### Parts
- Microcontroller - [Ardunio Nano Every](https://store-usa.arduino.cc/products/arduino-nano-every)
- Level Shifter (RS485 to TTL) - MAX488EPA+ - [Digikey](https://www.digikey.com/en/products/detail/analog-devices-inc-maxim-integrated/MAX488EPA/1495109?s=N4IgTCBcDaILIEEAaAWAHGgogBQQagAIQBdAXyA) | [Mouser](https://www.mouser.com/ProductDetail/Analog-Devices-Maxim-Integrated/MAX488EPA%2b?qs=1THa7WoU59G6dxfe6rTcAA%3D%3D)
- LED Ring - [NeoPixel 24x 5050 RGBW LED Ring](https://www.adafruit.com/product/1586)
- Connectors
  - Power - Anderson Powerpole 15/45
  - Communication - 5-pin M12 A-Code Circular Connectors [DigiKey](https://www.digikey.com/en/products/detail/conec/43-01199/2793477?s=N4IgTCBcDaIAQBYDMBaADARgwTmyAugL5A)/[Mouser](https://www.mouser.com/ProductDetail/Amphenol-CONEC/43-01199?qs=BLWaPj7617f34EH%2FcnQWlA%3D%3D)
