# Installing MQTT Broker
* Install MQTT

```
$ sudo apt update 
$ sudo apt install -y mosquitto
```  

* create file /etc/mosquitto/mosquitto.conf

```
$ sudo nano /etc/mosquitto/mosquitto.conf
```  

* write flie /etc/mosquitto/mosquitto.conf

```
pid_file /run/mosquitto/mosquitto.pid

persistence true
persistence_location /var/lib/mosquitto/

log_dest file /var/log/mosquitto/mosquitto.log

include_dir /etc/mosquitto/conf.d

# mqtt
listener 1883
protocol mqtt

# websockets
listener 9001
protocol websockets

allow_anonymous false
password_file /etc/mosquitto/passwd
```  

and save file (Ctrl+o for save and then Ctrl+x)

<img src="https://cdn.discordapp.com/attachments/1004952232145465354/1038034405765160970/image.png" alt='mqb' style="width:720px;height:405px;" >

## use MQTT Broker

```
$ sudo systemctl status mosquitto   #check MQTT Broker status
$ sudo systemctl start mosquitto.service   #active MQTT Brokker
$ sudo systemctl stop mosquitto.service   #inactive MQTT Broker
```  

<img src="https://cdn.discordapp.com/attachments/1004952232145465354/1038037436531490857/image.png" alt='mqb1' style="width:720px;height:405px;" >
