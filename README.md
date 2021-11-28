# Max7219-Clock
Desk Clock using MAX 7219 Led Based on Marqee Code  

This SW is baased on the Marquee project.
This is the opportunity form me to say Many Thanks fro realizing and sharing his project !!

This is the link to his project
https://github.com/Qrome/marquee-scroller

I have made some modification to try to improve it 

- Added MQTT control to do integreate it with Home Assistant (for example )
  - Display ON-OFF
  - Display Intensity

- Added Italian Languange
 
 
# MQTT Settings

To change MQTT parameter edit the Setting.h file

boolean ENABLE_MQTT = true;                   // this will allow you to comunicate to MQTT broker
const char* mqttServer = "KKK.YYY.ZZZ.XXX";   // Your MQTT server IP address
const char* mqttUser = "";                    // mqtt username, set to "" for no user
const char* mqttPassword = "";                // mqtt password, set to "" for no password
const char* mqtttopic = "ClockMatrix";        // mqtt topic

