# bruno-nano
Arduino UNO breakout board for NANO style MCU boards

![Board image](https://github.com/ole00/bruno-nano/raw/master/img/bruno-nano.jpg "bruno-nano")

This PCB allows you to experiment with various Arduino UNO shields while using an Arduino NANO style
board. The picture above uses a cheap LGT8F328P based NANO board.

NANO has - compared to UNO - two extra pins: A6 and A7. These are exposed to UNO pin header, next to
IOREF pin.

Capacitor C1 is a bypass capacitor for 5V rail, use 10 to 47uF capacitor or leave the footprint unpopulated.
Capacitor C2 is a bypass capacitor for 3.3V rail, use 10 to 47uF capacitor or leave the footprint unpopulated.

PCB version 1.1 (Rev 2) allows to select 5V or 3.3V IOREF voltage by using a jumper. Ensure your
IOREF voltage selection matches the MCU VCC. That is, if the MCU operates on 3.3V then select 3.3V IOREF
and if the MCU operates on 5V then select 5V IOREF. If unsure, then do not populate IOREF jumper at all.
Chances are the shield will not need the IOREF pin. Note that IOREF jumper does not magically
make your board 5V or 3.3V tolerant - IOREF pin is only used for IO voltage indication.
