# AttNo.de-powerpack, a adapter-pcb to use 3.3-15V
 AddOn to use the [attnode](https://attno.de) v2/v3 with 3.3-15V DC

This small pcb allows to run the [attnode](https://attno.de) with an operating voltage between 3.3 and 15V, for example with a USB power supply, a LiPo or any other fixed voltage power supply.

It has the shape of the CR2032 battery clip and is soldered directly onto the [attnode](https://attno.de) instead of the CR2032-Clip.

Therefore, when ordering the pcb's, a smaller pcb thickness can be used if possible, I have had good experiences with 1.2mm.

The power supply can be either via the JST socket, or the two pads directly on the pcb. In this case, the JST socket must not be soldered.

The voltage source must provide at least 120 mA.

Update 26.05.2021: add a Voltage divider added to monitor the Vin with an ADC pin of the ATTiny. The resistance ratio must be determined based on Vin, here are some sample values. The voltage at the ADC pad should not exceed 2.1V.

Update 27.08.2021: add two Resistors 5K1 and Pads for external wiring to support USB-C

  Vin | Vmax |  R1 | R2
------|------|-----|----
3.7V | 4.2V | 1M | 1M
USB | 5.25V | 1M5 | 1M
9V | 11V | 6M8 | 1M5
12V | 15.4V | 10M | 1M5

Attention! Pay attention to the peak voltage, which is higher than the nominal voltage for many batteries!

More information can be found [here](https://www.attno.de/blog/2021-01-08).

 front  | back       
--------|--------
![front view](https://raw.githubusercontent.com/theArcher73/attnode-powerpack/V1.2---USB-C/kicad-project/img/board_front.png) | ![Rear view](https://raw.githubusercontent.com/theArcher73/attnode-powerpack/V1.2---USB-C/kicad-project/img/board_rear.png)

## Disclaimer

The documentation of the attno.de-powerpack is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
