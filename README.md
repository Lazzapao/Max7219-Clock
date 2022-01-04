# Max7219-Clock

Desk Clock using MAX 7219 Led Based on Marqee Code  

This SW is baased on the Marquee project.
This is the opportunity for me to say Many Thanks for realizing and sharing his project !!

This is the link to his project:
https://github.com/Qrome/marquee-scroller

Refer to this web site for more info.
I have made some modification to try to improve it 

- Added MQTT control to do integreate it with Home Assistant (for example )
  - Display ON-OFF
  - Display Intensity

- Added Italian Languange
 
# MQTT Settings

To change MQTT parameter edit the Setting.h file

- boolean ENABLE_MQTT = true;                   // this will allow you to comunicate to MQTT broker
- const char* mqttServer = "KKK.YYY.ZZZ.XXX";   // Your MQTT server IP address 
- const char* mqttUser = "";                    // mqtt username, set to "" for no user
- const char* mqttPassword = "";                // mqtt password, set to "" for no password
- const char* mqtttopic = "ClockMatrix";        // mqtt topic


# Compiling and Loading to Wemos D1
It is recommended to use Arduino IDE. You will need to configure Arduino IDE to work with the Wemos board and USB port and installed the required USB drivers etc.

- USB CH340G drivers: https://sparks.gogo.co.nz/ch340.html
- Enter http://arduino.esp8266.com/stable/package_esp8266com_index.json into Additional Board Manager URLs field. You can add multiple URLs, separating them with commas. This will add support for the Wemos D1 Mini to Arduino IDE.
- Open Boards Manager from Tools > Board menu and install esp8266 Core platform version 2.7.4 DO NOT INSTALL 3.XX release or you will have compiling error !! 
- Select Board: "LOLIN(WEMOS) D1 R2 & mini"
- Set Flash Size to 4M (FS: 2MB OTA: 1019KB)
- Select the Port from the tools menu.


# 3D Printing files
Some Stl file are available in the stl-files folder.

![20211202_223655](https://user-images.githubusercontent.com/47435194/144507927-ab48e7e7-9345-4ebb-8f82-c96e7999d296.jpg)

This give the possibility to use any kind of PLA colours for printing the case and not only the light ones
Back plate is availaible in two release :

- Standard for D1 mini place only 
- Upgraded to a battery power Clock having USB-C port to recharge the battery
