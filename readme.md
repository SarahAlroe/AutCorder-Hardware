
Note: This is an early revision of the version 2 AutCorder hardware. Not ready for production. 

## Configuration jumpers 

- JP1 and JP2 provide options for enabling 3.3v on the last two pins of the FPC connector in either direction. This is for AF enabled OV5640 cameras. Untested, make sure pinout is correct. 
- JP3 Selects whether the battery voltage divider is constantly on or controlled by the PERIPH_PWR pin. To minimize battery consumption, always choose the latter. 

## Known issues 

- [ ] The POWERED_I voltage is too low on external power to wake the board. R5, a 100k resistor should be replaced with a 50k resistor to fix this. 
- [ ] Data transmission over the USB-C connector only works in one orientation, due to missing connectors. 
- [ ] JP3 should always bridge pins 1,2 
- [ ] Current FPC connector is too wide for the camera boards. Align carefully in the middle. 
- [ ] R10 should always be bridged. Remove in future version. 
- [ ] Physical space: J1 orientation makes the board significantly larger than necessary 
- [x] From V1 the replacement PDM microphone has tighter specifications, requiring a faster clock signal.  