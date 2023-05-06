## Lab 5 - Paho - MQTT

This lab uses MQTT a standard for sending information from one machine to another. This uses a two system dynamic with one being the publisher and one the subscriber.
This is managed by a broker which directs traffic from one system to another. This Lab creates two systems in the terminals, one a subscriber and one a publisher. 

## Lab Requirnments
This lab requires you to download Mosquito at teh following link " https://mosquitto.org/download/ "


## Steps 
1) The first step is to install Paho using the following command

            $ sudo pip3 install -U paho-mqtt
2) Next is to gitclone the eclipse paho.mqtt using the following commands  
 
             $ git clone https://github.com/eclipse/paho.mqtt.python.git 
            
3) Next direct to the file lesson 5 using the following command

             $ cd ~/iot/lesson5
             
4) Open up a second terminal and run the following command in both
    
             $ python3 subcpu.py
             
## Results
The reuslts and demonstration of this can be seen in the photo attached in this folder. One terminal is the publisher, sending data, and another terminal is the subscriber recieveing and outputing the data it recieves.
             
