# beatmania-IIDX-USKOC-Arduino-Leonardo

Conect your pad of beatmania IIDX USKOC to an Arduino Leonardo, the code is from [4yn](https://github.com/4yn/iivx)


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

## Acknowledgments:

]CrazyRedMachine's Ultimate Pop'n Controller](https://github.com/CrazyRedMachine/UltimatePopnController): PS2 Code/Handling
