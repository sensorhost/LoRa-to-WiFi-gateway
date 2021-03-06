# LoRa to WiFi gateway


### Introduction

The SensorHost LoRa to WiFi Gateway is a small device that provides connectivity between our LoRa sensors and your WiFi access point.
It is powered by a mains plug in power supply that provides 5volts DC. There are three indicator lights that provide the following information.
- Green (Power on)
- Blue (Wi-Fi operational status)
- Red (Wi-Fi activity)


### Requirements

- The gateway needs to be installed within range of your WiFi modem
- The gateway also needs to be located within range of your Lora sensors.
- The gateway connects to your WiFi access point using WPA2 security.


### Configuration - Connect to WiFi
- Connecting the gateway to your WiFi access point.
When the gateway has not been configured, it becomes an access point (AP) and the blue & red lights will flash alternately.

While in AP mode, you can use your smart device (phone/tablet/laptop) to connect to and configure the settings.
- On your smart device, look for an AP named LG01_AABBCCDD where `AABBCCDD` is part of the gateway key.
- Connect to this AP using `sensorhost` as the password.
- Once connected, open a web browser (Firefox or Chrome) and enter `42.42.42.42` in the address bar.
- The web page opens allowing you to set the WiFi credentials for your WiFi AP.
- Choose your WiFi AP, then enter it's password and then save the settings.
- The gateway will then reboot and connect to your WiFi AP and start operating.

Once the gateway has connected to your WiFi AP, the blue light should flash once every few seconds.
After 30-60 seconds, if the gateway blue light is flashing 3 times, you have most likely entered the wrong credentials for your WiFi access point to connect to. Please reset the gateway WiFi settings and start again.

### Configuration - Add gateway to your account
The gateway communicates with our server providing signal level information. For the gateway to operate normally, you need to add it to your account.
- Log into your account.
- Go to Manage->My sensor boxes.
- Click Add new sensorbox.
- Enter the gateway serial number and key.
- Save the changes.
Now if you go to the Manage->My sensor boxes section, you will the the gateway there and also any relevant information such as signal level etc.


#### Technical information
All our WiFi sensors use the following ports, if you have a firewall enabled you will need to allow these ports to be open.
- 80 (HTTP) used on startup to check the server is available.
- 8883 (MQTTS) secure MQTT, the sensors data is transferred over this port.


### Operation
Once the gateway is connected to your WiFi access point, there is little else to do.

### LoRa aerial
The standard gateway LoRa aerial (the small black one about 10cm long) only provides a limited range for the remote sensors. The range can vary depending on many factors. If you require greater range for your remote sensors please connect to an external LoRa antenna. In excess of 20km can be achieved with suitable aerials on both the gateway and sensor.

#### A note on range
It should be noted that when a range distance has been quoted it normally means 'line-of'sight'.

Put simply, 'line-of-sight' means if you were located at the gateway aerial, then you can see the sensor aerial (binoculars may be needed) but the key info here is that there is nothing between the two aerials except for free space.
