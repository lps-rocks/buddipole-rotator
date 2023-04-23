# buddipole-rotator

Inspired by [the rotator made by KI6AWR and HB9MTN](https://qsl.net/hb9mtn/BPMW/MW_Rotor.html), this rotator adds some additional features and makes some design changes. All of the rotator intelligence is located in the rotator at the mast and exposes an RS485 connection with the[Idiom Press Rotor-EZ Rotator Control Protocol](https://www.hamsupply.com/wp-content/uploads/2015/11/Rotor-EZ-Protocol.pdf).

I've split this into a few independent designs and parts

- Rotator
- Controller
- Wireless Module

## Rotator 

### Features
- All of the intelligence, control, and safety features are located in the Rotator. 
- The chosen Stepper motor driver has the ability to detect motor load, save power, and run cooler automatically
- Addition of an optical rotary encoder ensures safety of the components should the mast bind and stop rotating
- 

### Design
- Arduino Code - Link to Arduino Source Code
- Schematic - Link to Schematic
- Board - Link to board
- STL files - Link to STL files

### Parts
- Stepper [Nema 17 Bipolar 1.5A 42Ncm 42x42x38mm 1.8deg](https://www.amazon.com/STEPPERONLINE-Stepper-Bipolar-42x42x38mm-Connector/dp/B0B38GX54H)
- Stepper Driver - [SilentStepStick w/TMC2130](https://learn.watterott.com/silentstepstick/)
- Stepper Driver Protection - [SilentStepStick Protector](https://learn.watterott.com/silentstepstick/protector/)
- Rotary Encoder - [Optical Rotary Encoder 600P/R](https://www.amazon.com/gp/product/B085ZLCYS1/)
- Microcontroller - [Arduino Pro Mini (DEV-11113) from SparkFun](https://www.sparkfun.com/products/11113)
- Power Regulator - **TBD**

## 
