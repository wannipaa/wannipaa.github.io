# Learning to use Zigbee2MQTT

<img src="https://cdn.discordapp.com/attachments/1029328113932439572/1045760400802730064/unknown.png" alt='zb' style="width:200px;height:200px;" >

Zigbee2MQTT is a nodejs Gateway application that connects Zigbee networks to MQTT networks.  
(thx for infromation from: [here](https://stevessmarthomeguide.com/using-zigbee2mqtt-beginners-guide/#:~:text=Zigbee2MQTT%20is%20a%20nodejs%20Gateway,like%20the%20CC2531%20USB%20sniffer.))

## Installing on Ubuntu 
```
# Set up Node.js repository and install Node.js + required dependencies
# NOTE: Older i386 hardware can work with [unofficial-builds.nodejs.org](https://unofficial-builds.nodejs.org/download/release/v16.15.0/ e.g. Version 16.15.0 should work.
sudo curl -fsSL https://deb.nodesource.com/setup_16.x | sudo -E bash -
sudo apt-get install -y nodejs git make g++ gcc

# Verify that the correct nodejs and npm (automatically installed with nodejs)
# version has been installed
node --version  # Should output v14.X, V16.x, V17.x or V18.X
npm --version  # Should output 6.X, 7.X or 8.X

# Create a directory for zigbee2mqtt and set your user as owner of it
sudo mkdir /opt/zigbee2mqtt
sudo chown -R ${USER}: /opt/zigbee2mqtt

# Clone Zigbee2MQTT repository
git clone --depth 1 https://github.com/Koenkk/zigbee2mqtt.git /opt/zigbee2mqtt

# Install dependencies (as user "pi")
cd /opt/zigbee2mqtt
npm ci
```  
## Configuring
* Open the configuration file
```
$ nano /opt/zigbee2mqtt/data/configuration.yaml
```  
* write code
```
# MQTT settings
mqtt:
  # MQTT base topic for Zigbee2MQTT MQTT messages
  base_topic: zigbee2mqtt
  # MQTT server URL
  server: 'mqtt://localhost'
  # MQTT server authentication, uncomment if required:
  # user: my_user
  # password: my_password

# Serial settings
serial:
  # Location of the adapter (see first step of this guide)
  port: /dev/ttyACM0
```  
## Starting Zigbee2MQTT
```
cd /opt/zigbee2mqtt
npm start
```  
<img src="https://cdn.discordapp.com/attachments/1004952232145465354/1038036631074111539/image.png" alt='zb1' style="width:720px;height:405px;" >

Note: You have to has MQTT Broker before use Zigbee2MQTT  
Source:[Installation on Linux](https://www.zigbee2mqtt.io/guide/installation/01_linux.html)
