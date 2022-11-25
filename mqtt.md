# What is MQTT(´・ω・`)?
<img src="https://cdn.discordapp.com/attachments/1029328113932439572/1045735567524114543/unknown.png" alt='mq' style="width:286px;height:73px;" >

MQTT is an OASIS standard messaging protocol for the Internet of Things (IoT). It is designed as an extremely lightweight publish/subscribe messaging transport that is ideal for connecting remote devices with a small code footprint and minimal network bandwidth. MQTT today is used in a wide variety of industries, such as automotive, manufacturing, telecommunications, oil and gas, etc.  
(Thx for information from : [mqtt.org](https://mqtt.org/))

## How to install MQTT client package 

<img src="https://cdn.discordapp.com/attachments/1004952232145465354/1027889541832515654/unknown.png" alt='mq1' style="width:720px;height:405px;" >

<img src="https://cdn.discordapp.com/attachments/1004952232145465354/1027889658450939974/unknown.png" alt='mq2' style="width:720px;height:405px;" >

## Test MQTT Sever
* 1883: MQTT, unencrypted, unauthenticated
* 1884: MQTT, unencrypted, authenticated
* 8883: MQTT, encrypted, authenticated
* 8884: MQTT, unencrypted, client certificate required
* 8885: MQTT, encrypted, authenticated
* 8886: MQTT, encrypted, unauthenticated
* 8887: MQTT, encrypted, sever certificate deliberately expired
* 8080: MQTT over WebSockets, unencrypted, unauthenticated
* 8081: MQTT over WebSockets, encrypted, unauthenticated
* 8090: MQTT over WebSockets, unencrypted, authenticated
* 8091: MQTT over WebSockets, encrypted, unauthenticated  
Source:[https://test.mosquitto.org](https://test.mosquitto.org)

## let's try it!!
### In Ubuntu
Use port 1883

<img src="https://cdn.discordapp.com/attachments/1029328113932439572/1031841077054951456/unknown.png" alt='mq3' style="width:720px;height:405px;" >

### In RPi OS
Use port 1883

<img src="https://cdn.discordapp.com/attachments/1029328113932439572/1031843768137158666/unknown.png" alt='mq4' style="width:720px;height:405px;" >
