# Compilation procedure for WSPR-TX 1.14 

## Install Arduino IDE

See [Getting started with the Arduino products](https://www.arduino.cc/en/Guide)

## Before compilation

In the Arduino IDE, do the following:

* Set board to `Arduino Pro or Pro Mini`
* Set processor to `ATMega328P (3.3V, 8MHz)`
* Install library `NeoGPS by Slash Devin` at yhe library manageri
* locate and modify the file `NMEAGPS_cfg.h`. It is a part of the NeoGPS library. The path on macOS is: `~/Documents/Arduino/libraries/NeoGPS/src`
* Enable the following flags in `NMEAGPS_cfg.h` by uncommenting them:

```c++
#define NMEAGPS_PARSE_GSV
#define NMEAGPS_PARSE_SATELLITE_INFO
#define NMEAGPS_PARSE_SATELLITES
```

## How to compile and write the result

* Open the file "WSPR-TX1.14.ino"
* Verify and upload compiled binary

