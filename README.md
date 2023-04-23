# buddipole-rotator

Inspired by [the rotator made by KI6AWR and HB9MTN](https://qsl.net/hb9mtn/BPMW/MW_Rotor.html) this rotator adds some additional features and makes some design changes. 

I've split this into a few independent designs and parts

- Rotator
- Controller
- Wireless Adapter

## Rotator 

### Design
- All stepper controls / intelligence is at the mast
- RS485 Control compliant with [Idiom Press Rotor-EZ Rotator Control Protocol](https://www.hamsupply.com/wp-content/uploads/2015/11/Rotor-EZ-Protocol.pdf)

### Parts
- Stepper Driver - [SilentStepStick w/TMC2130](https://learn.watterott.com/silentstepstick/) w/TMC2130 stepper driver
- Stepper Driver Protection - [SilentStepStick Protector](https://learn.watterott.com/silentstepstick/protector/)
- Rotary Encoder - [Optical Rotary Encoder 600P/R](https://www.amazon.com/gp/product/B085ZLCYS1/)
- Microcontroller - [Arduino Pro Mini (DEV-11113) from SparkFun](https://www.sparkfun.com/products/11113)
- Power Regulator [TBD]

## Rotator Additional Features
- RS485 to Digi XBee3 for Wireless control
