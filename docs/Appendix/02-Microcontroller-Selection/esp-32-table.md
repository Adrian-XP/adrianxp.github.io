P---
title: Appendix - Controller Table for the ESP32
---

| ESP Info                                      | Answer |
| --------------------------------------------- | ------ | 
| Model                                         | ESP32=S3      |
| Product Page URL                              | Found in [Expressif.com](https://www.espressif.com/en/products/socs/esp32-s3)      |
| ESP32-S3-WROOM-1-N4 Datasheet URL             | [link](https://documentation.espressif.com/esp32-s3-wroom-1_wroom-1u_datasheet_en.pdf)      | 
| ESP32 S3 Datasheet URL                        | [link](https://documentation.espressif.com/esp32-s3_datasheet_en.pdf)      |
| ESP32 S3 Technical Reference Manual URL       | [link](https://documentation.espressif.com/esp32-s3_technical_reference_manual_en.pdf)      | 
| Vendor link                                   | Digikey [link](https://www.digikey.com/en/products/detail/espressif-systems/ESP32-S3-WROOM-1-N4/16162639)      |
| Code Examples                                 | [SD Card Detect](https://docs.sparkfun.com/SparkFun_Thing_Plus_ESP32-S3/arduino_example/#sd-card-detect), [I2C Scanner Power Control](https://docs.sparkfun.com/SparkFun_Thing_Plus_ESP32-S3/arduino_example/#i2c-scanner-power-control)      |
| External Resources URL(s)                     | [A beginner’s guide to ESP32](https://www.youtube.com/watch?v=UuxBfKA3U5M)      | 
| Unit cost                                     | $5.06      | 
| Absolute Maximum Current for entire IC        | 800 mA      | 
| Supply Voltage Range                          | min - 3V, nominal - 3.3V, max - 3.6V      | 
| Absolute Maximum current <br> (for entire IC) | 600 mA      | 
| Maximum GPIO current <br> (per pin)           |  40 mA     | 
| Supports External Interrupts?                 | Yes      | 
| Required Programming Hardware, Cost, URL      | [link](https://docs.espressif.com/projects/esp-idf/en/latest/esp32s3/get-started/index.html)      | 


| Module         | # Available | Needed | Associated Pins (or * for any) |
| -------------- | ----------- | ------ | ------------------------------ |
| UART           | 3           | 1      | Any GPIO Pin                              |
| external SPI\* | 3           | 1-2      | Any GPIO Pin                              |
| I2C            | 2           | 1-2      | Any GPIO Pin                             |
| GPIO           | 44           | 5      | Any GPIO Pin                             |
| ADC            | 2 ADC, 20 Channels           | 0      | IO pin 1-20                              |
| LED PWM        | 8           | 0      | Any GPIO Pin                             |
| Motor PWM      | 2           | 0      | Any GPIO Pin                             |
| USB Programmer | 1           | 1      | GPIO 19, 20                              |

The ESP32-S3 is much more powerful than the PIC18F47K42, thanks to its speed and features. While the PIC chip runs at only 64 MHz, the ESP32-S3 has two cores that run up to 240 MHz. This means it can handle many tasks simultaneously very quickly. The ESP32-S3 also has 512 KB of memory, which is much larger than the PIC's. One of the biggest wins is that the ESP32-S3 has built-in Wi-Fi and Bluetooth. The PIC chip does not have these, so it cannot communicate with the internet or phones on its own and needs the SNAP. In addition, there is no need to use MPLAB when using the ESP32-S3, as it has issues with MCC; making the ESP32-S3 is a better choice.

