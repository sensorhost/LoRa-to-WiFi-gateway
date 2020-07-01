# LoRa to WiFi gateway


### Introduction

The SensorHost LoRa to WiFi Gateway is a small device that provides connectivity between our LoRa sensors and your WiFi access point.
It is powered by a mains plug in power supply that provides 5volts DC. There are four indicator lights that provide the following information.
- Green (Power on)
- Blue (Wi-Fi operational status)
- Red (Wi-Fi activity)
- Yellow (LoRa activity)


### Requirements

- The gateway needs to be installed within range of your WiFi modem
- The gateway also needs to be located within range of your Lora sensors.


### Configuration
- Connecting the gateway to your WiFi access point.
When the gateway has not been configured, it becomes an access point (AP) and the blue & red lights will flash alternately.

While in AP mode, you can use your smart device (phone/tablet/laptop) to connect to and configure the settings.
- On your smart device, look for an AP named LG01_AABBCCDD where `AABBCCDD` is part of the gateway key.
- Connect to this AP using `sensorhost` as the password.
- Once connected, open the web browser and enter `42.42.42.42` in the address bar.
- The web page opens allowing you to set the WiFi credentials for your WiFi AP.
- Choose your WiFi AP, then enter it's password and then save the settings.
- The LG01 will then reboot and connect to your WiFi AP and start operating.

