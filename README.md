## PlatformIO IDE ESP-IDF ESP32 ESP-MQTT example
## Adafruit IO

I used: 
- Simple library for single DS18B20 on ESP32 https://github.com/feelfreelinux/ds18b20
- ESP-MQTT sample application https://github.com/espressif/esp-idf/tree/master/examples/protocols/mqtt/tcp

This code sends data every 10 seconds on io.adafruit.com.
I used ds18b20 to get temperature and send it.

## You need to set next parametrs:
- **DS_PIN** - GPIO where you connected ds18b20
- **WIFI_SSID** - SSID of your WIFI network
- **WIFI_PASS** - password of your WIFI network
- **BROKER_URL** - mqtt://login:aio_xxx@io.adafruit.com
    - where 
    - login - Your AdafruitIO Username
    - aio_xxx - Your AdafruitIO Key
- **IO_TOPIC** login/feeds/name_feed
    - where
    - login - Your AdafruitIO Username
    - name_feed - Your AdafruitIO Feed name
