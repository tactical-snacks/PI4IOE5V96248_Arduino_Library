# PI4IOE5V96248_Arduino_Library
Arduino Library for PI4IOE5V96248
This chip is an I2C IO expander chip, with 48 I/O pins configurable over I2C.
The library is really basic, mostly using the Wire library. It is made just to provide some convenience functions for users.

### Note: This chip defaults to all pins HIGH on power on. This is expected since it's mostly designed as a LED driver chip, but good to note.
Pins must be left HIGH for input sensing. External circuitry may then pull the pin LOW, and reads will correctly reflect the pin state.

## Installation:
Download the .zip file from Github, in Arduino go to Sketch -> Include Library -> Add .ZIP Library... and select the downloaded .zip file.  
The library example can then be opened under File -> Examples -> PI4IOE5V96248 IO Expander  

Software is licensed under BSD 3 Clause: https://opensource.org/licenses/BSD-3-Clause   
Documentation is licensed under Attribution-ShareAlike 2.0 Generic (CC BY-SA 2.0): https://creativecommons.org/licenses/by-sa/2.0/   
All rights reserved by Blueprint Foundry.

# Fork Notes

## Changes from Upstream

### Added
- extended pin mapping for pin read and write
- i2c address table

### Fixed
- readAll compiler warning

### Changed
- Corrected README input read documentation