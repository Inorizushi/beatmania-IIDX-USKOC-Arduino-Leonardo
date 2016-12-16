# beatmania-IIDX-USKOC-Arduino-Leonardo

Conect your pad of beatmania IIDX USKOC to an Arduino Leonardo


##Hardware

####Arduino
You can buy an Arduino Leonardo from [Ebay](http://www.ebay.com/) or [AliExpress](http://www.aliexpress.com), unless you want an original version [Arduino.cc](https://www.arduino.cc/en/Guide/ArduinoLeonardoMicro)

####Quadrature Encoder
The encoder or scarth from your USKOC beatmania pad will look like this.
http://imgur.com/K6XgcYp
Reverse http://imgur.com/lrmyJkw

So to connect the the quadrature encoder into the arduino, is necesary make the following setup.
http://imgur.com/kNGvjr9

(Work in progres)

## Wiring

leoo.ino uses the following pins:

| Item                    | Pin |
|-------------------------|-----|
| **Buttons**             |     |
| Btn 1 Switch            | A0  |
| Btn 2 Switch            | A1  |
| Btn 3 Switch            | A2  |
| Btn 4 Switch            | A3  |
| Btn 5 Switch            | A4  |
| Btn 6 Switch            | A5  |
| Btn 7 Switch            | 13  |
| Btn 8 Switch (Star)     | 12  |
| Btn 9 Switch (Select)   | 11  |
| **Encoders**            |     |
| Turntable Enc Channel A |  0  |
| Turntable Enc Channel B |  1  |


