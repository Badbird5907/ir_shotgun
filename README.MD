# IR Shotgun
This is a IR shotgun (blaster) for the flipper zero that uses 8x APTD3216F3C-P22 infrared LEDs to absolutely FLOOD a room with infrared light.

## How does it work?
The flipper zero drives the A7 pin with PWM, which in turn drives the AO3400A MOSFET. The MOSFET then turns on and off the IR LEDs.

## How does this compare to the Rabbit Labs IR Blaster?
This blaster is (I think) a bit more powerful, and more directional compared to the Rabbit Labs IR Blaster.

## Design choices
- Instead of using 1x3 pin headers, I used 2x3 headers to provide better structural support for the blaster PCB.
- I used the AO3400A MOSFET over the 2N7000 because it's able to handle more current.
- My calculations for the resistor values for the LEDs (70 ohm -> 68 ohm) were based on the DC Forward Current of 50mA and not the peak forward current of 1200mA.

## Pictures
![render](https://cdn.badbird.dev/screenshots/2025/07/KPPCeMie5l.png)
![blaster back](https://cdn.badbird.dev/screenshots/2025/07/K4bML5AEqf.png)
![blaster](https://cdn.badbird.dev/screenshots/2025/07/qfoLDu9WEQ.png)
![base](https://cdn.badbird.dev/screenshots/2025/07/YxU8aKaOy6.png)

## BOM
|Name                                                                                                                       |Qty   |Price Per (USD)|Total (USD)|Link                                                                                       |
|---------------------------------------------------------------------------------------------------------------------------|------|---------------|-----------|-------------------------------------------------------------------------------------------|
|90 Degree header                                                                                                           |1     |$0.67          |$0.67      |https://www.digikey.ca/en/products/detail/w%C3%BCrth-elektronik/61300621021/4846834        |
|0.1uF 0805 cap                                                                                                             |1     |$0.08          |$0.08      |https://www.digikey.ca/en/products/detail/samsung-electro-mechanics/CL21B104KBCNNNC/3886661|
|10uF 1206 cap                                                                                                              |1     |$0.08          |$0.08      |https://www.digikey.ca/en/products/detail/samsung-electro-mechanics/CL31B106KAHNNNE/3887462|
|IR LED                                                                                                                     |8     |$0.52          |$4.16      |https://www.digikey.ca/en/products/detail/kingbright/APTD3216F3C-P22/8591562               |
|AO3400A MOSFET                                                                                                             |1     |$0.46          |$0.46      |https://www.digikey.ca/en/products/detail/alpha-omega-semiconductor-inc/AO3400A/1855772    |
|68 ohm res                                                                                                                 |4     |$0.60          |$2.40      |https://www.digikey.ca/en/products/detail/susumu/HRG3216P-68R0-D-T1/5762544                |
|10k res                                                                                                                    |1     |$0.10          |$0.10      |https://www.digikey.ca/en/products/detail/stackpole-electronics-inc/RMCF0805FT10K0/1760676 |
|15mm pin headers                                                                                                           |1     |$3.43          |$3.43      |https://www.aliexpress.com/item/1005006783391171.html                                      |
|Blaster PCB (JLC, LeadFree HASL)                                                                                           |1     |$5.20          |$5.20      |                                                                                           |
|Base PCB (JLC, LeadFree HASL)                                                                                              |1     |$5.20          |$5.20      |                                                                                           |
|TOTAL                                                                                                                      |      |               |$21.78     |                                                                                           |
|NOTE: Most of the resistors/caps here cost more in packages of one than in packages of 10+, I'd suggest ordering 10 of each|      |               |           |                                                                                           |
|                                                                                                                           |      |               |           |                                                                                           |
|                                                                                                                           |USD   |               |           |                                                                                           |
|JLC - DHL                                                                                                                  |$17.50|               |           |                                                                                           |
|DigiKey                                                                                                                    |$5.84 |               |           |                                                                                           |
|                                                                                                                           |      |               |           |                                                                                           |
|                                                                                                                           |      |               |           |                                                                                           |
|Grand Total                                                                                                                |      |               |$45.12     |                                                                                           |
                                                                                  |      |               |           |                                                                                           |
|Shipping
