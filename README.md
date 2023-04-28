# buddipole-rotator

Inspired by [the rotator made by KI6AWR and HB9MTN](https://qsl.net/hb9mtn/BPMW/MW_Rotor.html), this rotator adds some additional features and makes some design changes. All of the rotator intelligence is located in the rotator at the mast and exposes an RS485 connection with the [Idiom Press Rotor-EZ Rotator Control Protocol](https://www.hamsupply.com/wp-content/uploads/2015/11/Rotor-EZ-Protocol.pdf).

I've split this into a few independent designs and parts

- Rotator
- Controller
- Wireless Module

## Rotator 

### Features
- Utilizes [Idiom Press Rotor-EZ Rotator Control Protocol](https://www.hamsupply.com/wp-content/uploads/2015/11/Rotor-EZ-Protocol.pdf) over Full Duplex RS-485 via 5-pin 16mm aviation connector
- Trinamic TMC2130 Stepper driver can intelligently adjust power output to the stepper based on load to prevent lost steps, maximize motor torque, reduce power consumption, and heat output
- Can operate off of wide voltage range
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
- Microcontroller - [SparkFun Arduino Pro Mini (DEV-11113)](https://www.sparkfun.com/products/11113)
- Level Shifter for RS485 Communication - MAX488 Chip (Full Duplex RS485 w/reduced EMI)
- Power Regulator - **TBD**
- Connectors
  - Power - Anderson Powerpole 15/45
  - Communication - 16mm 5 pin aviation connector 

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
- TBD
