# Plant Moisture Sensor

## Hardware Requirements
* ESP8266 board: https://www.amazon.com/HiLetgo-Internet-Development-Wireless-Micropython/dp/B081CSJV2V/ref=sr_1_4?dchild=1&keywords=ESP8266&qid=1622662260&sr=8-4
* Adafruit STEMMA soil sensor: https://www.adafruit.com/product/4026

## Software Requirements
* PlatformIO CLI: https://docs.platformio.org/en/latest/core/index.html
  * `brew install platformio`

Project created with PlatformIO CLI via `pio project init --ide vim --board nodemcuv2`

## PlatformIO Board Info
* Board: ESP8266 NodeMCU CP2102 ESP-12E built by HiLetGo
* Platform: espressif8266
* nodemcuv2          ESP8266  80MHz        4MB      80KB   NodeMCU 1.0 (ESP-12E Module)

## PlatformIO basic commands

Build what's in /src and upload to the ESP8266:
```
platformio run --target upload
```

Watch serial output from Serial.write:
```
platformio device monitor
```

Install a lib:
```
pio lib install "adafruit/Adafruit seesaw Library@^1.4.3"
```

Or maniually via `platformio.ini`:
```
lib_deps =
  adafruit/Adafruit seesaw Library @ ^1.4.3
```

## I2C

* https://diyi0t.com/what-is-the-esp8266-pinout-for-different-boards/
* https://diyi0t.com/i2c-tutorial-for-arduino-and-esp8266/

* "SDA (serial data) wire is used for data exchange between master and slave devices. SCL (serial clock) is used for the synchronous clock in between master and slave devices."
* SDA = data = pin D2 = white wire
* SCL = clock = pin D1 = green wire

## Board Links:

* https://www.amazon.com/gp/product/B081CSJV2V/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&th=1
* http://www.hiletgo.com/ProductDetail/1997591.html
* https://docs.platformio.org/en/latest/platforms/espressif8266.html
* https://github.com/nodemcu/nodemcu-firmware/tree/dev-esp32
* https://github.com/nodemcu/nodemcu-devkit-v1.0
* https://nodemcu.readthedocs.io/en/dev-esp32/
* https://github.com/platformio/platform-espressif8266/tree/master/examples/arduino-blink?utm_source=platformio.org&utm_medium=docs
* https://github.com/platformio/platform-espressif8266/tree/master/examples/esp8266-rtos-sdk-blink?utm_source=platformio.org&utm_medium=docs
* http://www.hiletgo.com/ProductDetail/2165564.html
* https://github.com/espressif?q=esp8266&type=&language=&sort=
* https://www.electronicwings.com/nodemcu/nodemcu-i2c-with-arduino-ide

## Soil Sensor Links:
* https://www.adafruit.com/product/4026
* https://learn.adafruit.com/adafruit-stemma-soil-sensor-i2c-capacitive-moisture-sensor
* https://learn.adafruit.com/adafruit-stemma-soil-sensor-i2c-capacitive-moisture-sensor/arduino-test

