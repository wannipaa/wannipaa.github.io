# Let's get to know Node-RED!!!
<img src="https://cdn.discordapp.com/attachments/1029328113932439572/1045754660461482055/unknown.png" alt='nr' style="width:286px;height:286px;" >

### Node-RED is....
Node-RED is a programming tool for wiring together hardware devices, APIs and online services in new and interesting ways.  
It provides a browser-based editor that makes it easy to wire together flows using the wide range of nodes in the palette that can be deployed to its runtime in a single-click.  
(Thx for information from: [nodered.org](https://nodered.org/))

## How to install Node-RED on Ubuntu
* Install curl and Node (v16.x)  
```
$ sudo apt install -y curl
$ curl -fsSL https://deb.nodesource.com/setup_16.x | sudo -E bash -
$ sudo apt install -y nodejs
```  
* Instal Node-RED locally
```
$ sudo npm install -g --unsafe-perm node-red
$ node-red
```  
* Or using a docker container
```
$ docker run -it -p 1880:1880 -v $HOME/ .node-red:/data --name mynodered nodered/node-red
```  
* Open in the browser: http://127.0.0.1:1880  
(thx for information from  
: [https://nodered.org/docs/getting-started/local](https://nodered.org/docs/getting-started/local)  
: [https://nodered.org/docs/getting-started/docker](https://nodered.org/docs/getting-started/docker))

## Let's try it!!!

* Test 1

<img src="https://cdn.discordapp.com/attachments/1004952232145465354/1032902199648468992/unknown.png" alt='nr1' style="width:720px;height:405px;" >

<img src="https://cdn.discordapp.com/attachments/1004952232145465354/1032902340707106826/unknown.png" alt='nr2' style="width:720px;height:405px;" >

<img src="https://cdn.discordapp.com/attachments/1004952232145465354/1032902436819578950/unknown.png" alt='nr3' style="width:720px;height:405px;" >

* Test 2 (with MQTT)

<img src="https://cdn.discordapp.com/attachments/1004952232145465354/1032921526028206090/unknown.png" alt='nr4' style="width:720px;height:405px;" >

<img src="https://cdn.discordapp.com/attachments/1004952232145465354/1032918973748084796/unknown.png" alt='nr5' style="width:720px;height:405px;" >

<img src="https://cdn.discordapp.com/attachments/1004952232145465354/1032920084781477918/unknown.png" alt='nr6' style="width:720px;height:405px;" >

<img src="https://cdn.discordapp.com/attachments/1004952232145465354/1032920137369669652/unknown.png" alt='nr7' style="width:720px;height:405px;" >

<img src="https://cdn.discordapp.com/attachments/1004952232145465354/1032920280789696572/unknown.png" alt='nr8' style="width:720px;height:405px;" >

<img src="https://cdn.discordapp.com/attachments/1004952232145465354/1032920368098332762/unknown.png" alt='nr9' style="width:720px;height:405px;" >

<img src="https://cdn.discordapp.com/attachments/1004952232145465354/1032921469216362536/unknown.png" alt='nr10' style="width:720px;height:405px;" >

* Test 3 (with MQTT and Send message)

<img src="https://cdn.discordapp.com/attachments/1004952232145465354/1032916408788590624/unknown.png" alt='nr11' style="width:720px;height:405px;" >

<img src="https://cdn.discordapp.com/attachments/1004952232145465354/1032917191697383444/unknown.png" alt='nr12' style="width:720px;height:405px;" >

<img src="https://cdn.discordapp.com/attachments/1004952232145465354/1032917336879022100/unknown.png" alt='nr13' style="width:720px;height:405px;" >

<img src="https://cdn.discordapp.com/attachments/1004952232145465354/1032917632275447808/unknown.png" alt='nr14' style="width:720px;height:405px;" >

<img src="https://cdn.discordapp.com/attachments/1004952232145465354/1032917745358078032/unknown.png" alt='nr15' style="width:720px;height:405px;" >

<img src="https://cdn.discordapp.com/attachments/1004952232145465354/1032917851046150185/unknown.png" alt='nr16' style="width:720px;height:405px;" >

<img src="https://cdn.discordapp.com/attachments/1004952232145465354/1032920084781477918/unknown.png" alt='nr17' style="width:720px;height:405px;" >

<img src="https://cdn.discordapp.com/attachments/1004952232145465354/1032920368098332762/unknown.png" alt='nr18' style="width:720px;height:405px;" >
