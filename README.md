# Arduino Nano Clone LGT8F328P

### LGT8F328P - Enhanced Arduino-Compatible Microcontroller

The **LGT8F328P** is a powerful microcontroller designed as an Arduino clone with enhanced features and better specifications than the widely used ATmega328P. It is fully compatible with the Arduino IDE and offers a range of improvements, making it ideal for more demanding electronics projects.

#### Key Features:
- **Faster Clock Speed**: Operates at up to 32 MHz (compared to the ATmega328P's 20 MHz)
- **Internal Oscillator**: 32 MHz internal clock for precise timing and improved performance
- **PWM and Timers**: 9 PWM channels (vs 6) and multiple timers with a frequency of up to 64 MHz
- **Analog Features**: 12-bit ADC channels with differential measurement support and selectable gain (1x, 8x, 16x, 32x)
- **DAC Output**: Integrated 8-bit DAC for real analog output
- **Extended EEPROM**: Simulated EEPROM with 0/1/2/4/8 KB options, using flash memory
- **Higher GPIO Current**: Up to 30 mA per pin, with special high-current GPIOs that can handle up to 80 mA

#### Why Choose LGT8F328P?
The LGT8F328P offers better performance, more flexibility in analog and digital capabilities, and higher speed, all while maintaining full compatibility with the Arduino environment. It's the perfect choice for anyone looking to push the limits of their DIY electronics projects without sacrificing ease of use.

---

### Comparison between ATmega328P VS LGT8F328P


| Feature                        | LGT8F328P                                          | ATmega328P                                      |
|---------------------------------|---------------------------------------------------|-------------------------------------------------|
| **System clock**                | Up to 32 MHz: ≤ 32 MHz @ 1.8 - 5.5V               | Up to 20 MHz: ≤ 4 MHz @ 1.8 - 5.5V <br> ≤ 10 MHz @ 2.7 - 5.5V <br> ≤ 20 MHz @ 4.5 - 5.5V |
| **Internal oscillator**         | 32 MHz                                            | 8 MHz                                           |
| **Timer**                       | 2 x 8 Bit, 2 x 16-Bit <br> Frequency up to 64 MHz | 2 x 8-Bit, 1 x 16-Bit <br> Frequency up to 20 MHz |
| **PWM channels**                | 9 channels (QFP32L: 8 channels)                   | 6 channels                                      |
| **ADC channels**                | 12 channels, up to 12-bit resolution <br> Gain: 1x, 8x, 16x, 32x <br> Differential measurement option | 8 Channels, 10-bit resolution <br> No gain <br> No differential measurements (single-ended only) |
| **"Real" DAC output**           | DAC with resolution of 8 bit                      | No DAC                                          |
| **Int. reference voltages**     | 1.024 V, 2.048 V, 4.096 V +/- 1%                  | 1.1 V +/- 0.1 V                                 |
| **EEPROM**                      | "Simulated" EEPROM at the cost of flash <br> 0/1/2/4/8 KB (1 KB EEPROM uses 2 KB Flash) | 1 KB EEPROM                                     |
| **GPIO current**                | Up to 30 mA <br> 6 GPIOs can supply 80 mA (QFP32L: 4 GPIOs) | Up to 40 mA, recommended: ≤ 20 mA <br> No "high-current" outputs |


---

This developing board can be fabricated in home a printable file is attached in PCB folder.

## 2D PCB
![2D PCB](https://github.com/AhmedHafez2000/Arduino-Nano-Clone-LGT8F328P/blob/main/PCB/2D-Top.png?raw=true)
**NOTE:** The bottom connection are jumper wires.

## 3D PCB
![3D PCB](https://github.com/AhmedHafez2000/Arduino-Nano-Clone-LGT8F328P/blob/main/PCB/3D-Top.png?raw=true)

## DIY Sample
![](https://github.com/AhmedHafez2000/Arduino-Nano-Clone-LGT8F328P/blob/main/Photos/IMG_1.jpg?raw=true)
![](https://github.com/AhmedHafez2000/Arduino-Nano-Clone-LGT8F328P/blob/main/Photos/IMG_2.jpg?raw=true)
![](https://github.com/AhmedHafez2000/Arduino-Nano-Clone-LGT8F328P/blob/main/Photos/IMG_3.jpg?raw=true)


The LGT8F328P IC that I am using has already arduino bootloader so to make design easier I removed bootloader pins.

The design is inspired by the following developing board:

![](https://github.com/AhmedHafez2000/Arduino-Nano-Clone-LGT8F328P/blob/main/Ref/lgt8f328p_nano_qfp32l_pinout.jpg?raw=true)

## Settings:
![](https://github.com/AhmedHafez2000/Arduino-Nano-Clone-LGT8F328P/blob/main/Photos/1.png?raw=true)
First install LGT8fx Boards

![](https://github.com/AhmedHafez2000/Arduino-Nano-Clone-LGT8F328P/blob/main/Photos/2.png?raw=true)
Then select the board

![](https://github.com/AhmedHafez2000/Arduino-Nano-Clone-LGT8F328P/blob/main/Photos/3.png?raw=true)
and choose operating frequency

![](https://github.com/AhmedHafez2000/Arduino-Nano-Clone-LGT8F328P/blob/main/Photos/4.png?raw=true)
and choose the model used

![](https://github.com/AhmedHafez2000/Arduino-Nano-Clone-LGT8F328P/blob/main/Photos/5.png?raw=true)
The upload speed that work for me is 115200.


