# beatmania-IIDX-USKOC-Arduino-Leonardo

Connect your pad of beatmania IIDX USKOC to an Arduino Leonardo, the code is from [4yn](https://github.com/4yn/iivx)

## Differences from Hormash's Repo
- Changed pinouts to make more sense.
- Added PS2 compatibility. (Thank you CrazyRedMachine)
- Adjusted TT Sensitivity.

## Hardware

#### Arduino
You can buy an Arduino Leonardo from [Ebay](http://www.ebay.com/) or [AliExpress](http://www.aliexpress.com), unless you want an original version [Arduino.cc](https://www.arduino.cc/en/Guide/ArduinoLeonardoMicro)

#### Quadrature Encoder
The encoder or scarth from your USKOC beatmania pad will look like this [IMG 1](http://imgur.com/K6XgcYp) reverse [IMG2](http://imgur.com/lrmyJkw)

So to connect the the quadrature encoder into the arduino, is necesary make the following [setup](https://imgur.com/NbJVJxu)

(Work in progres)

## Wiring

leoo.ino uses the following pins:

| Item                    | Pin |
|-------------------------|-----|
| **Buttons**             |     |
| Btn 1 Switch            |  2  |
| Btn 2 Switch            |  3  |
| Btn 3 Switch            |  4  |
| Btn 4 Switch            |  5  |
| Btn 5 Switch            |  6  |
| Btn 6 Switch            |  7  |
| Btn 7 Switch            |  8  |
| Btn 8 Switch (Start)    |  9  |
| Btn 9 Switch (Select)   | 10  |
| **LEDs**                |     |
| Btn 1 LED               |  11 |
| Btn 2 LED               |  12 |
| Btn 3 LED               |  13 |
| Btn 4 LED               |  A0 |
| Btn 5 LED               |  A1 |
| Btn 6 LED               |  A2 |
| Btn 7 LED               |  A3 |
| Btn 8 LED (Start)       |  A4 |
| Btn 9 LED (Select)      |  A5 |
| **Encoders**            |     |
| Turntable Enc Channel A |  0  |
| Turntable Enc Channel B |  1  |

## Playstation compatibility
(From CrazyRedMachine's Ultimate Pop'n Controller)
Arduino Leonardo version is also compatible with Playstation and Playstation 2 (it can be made to be plugged directly to the controller port, using the following pinout).

![pinout_psx](https://github.com/CrazyRedMachine/UltimatePopnController/blob/master/pinout_leonardo_psx.png?raw=true)

For ACK (TXLED aka PD5) and SS (RXLED aka PB0) you have to solder new headers or cables directly on the leonardo PCB (or you can use an Arduino Micro (not pro micro) which has everything broken out).

LEDs will be dimmer due to 3.3v power. Using the 7V rumble motor line to Vin instead, and using NPN transistors like 2N2222A on MISO and ACK lines to prevent backfeeding voltage into the console will solve the issue (set INVERT_CIPO and INVERT_ACK to 1 in `ps2.c`).

**BEWARE: DO NOT PLUG USB AND PSX AT THE SAME TIME, THIS CAN DAMAGE YOUR CONSOLE**

## Acknowledgments:

[CrazyRedMachine's Ultimate Pop'n Controller](https://github.com/CrazyRedMachine/UltimatePopnController): PS2 Code/Handling
