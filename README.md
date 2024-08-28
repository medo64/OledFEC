# OLED Framework Expansion Card

Framework computer expansion card that allows a USB CDC serial connection to
SSD1306 OLED display modules.


## Pinout

To connect to this board, one has to use a 4-pin JST XH connector. The following
table represents the pinout, pin 1 being on the left as looking into the
expansion card.

| # | Ref   | Description                     |
|--:|:-----:|---------------------------------|
| 1 | GND   | Ground connection               |
| 2 | 5V    | OLED power                      |
| 2 | SCL   | I²C clock                       |
| 3 | SDA   | I²C data                        |

As power consumption is low, wires can be almost any AWG. I would recommend
using 24 AWG wire 0.25 mm² as they allow for greater compatibility with other
connectors.


## LEDs

LED will blink on UART communication with computer (both sending toward and
receiving data from computer).


## Protocol

This driver will present itself to the system as CDC USB device. Communication
protocol is text-based and available [here](https://github.com/medo64/UsbOled.Firmware).


---

*You can check my blog and other projects at [www.medo64.com](https://www.medo64.com/electronics/).*
