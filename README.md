
# Home automation and security through IoTs  

This is a ESP32  and Blynk based project. Those pople who have small kids at home face home invasion and didn't know it until they reach home, even with Ring Door bell you can't tell whether your door is being opened or not. But using this device we can know the state of the gate, the user will get the update in his Blynk application whenever the gate state changes.
There is a MQ2 sensor which is capable of detecting the smoke/LPG leakage in the house.It also display the live smoke/LPG level through a circular guage over blynk application once the smoke/LPG level is above threshold value it can sound a buzzer and sends a warning message to the user's mobile.
It has the ability to control two home appliances, if there is no internet connectivity in the ESP32 than with two push buttons the appliances can be toggled and once the connectivity is established their states will be updated over the blynk application.
## Features

- Live notification of door
- Live Smoke/LPG leakage indication
- Automate two home appliance
- Works both online and offline
- Get notification even when the Blynk is closed
## Deployment

To deploy this project run

add Auth Token from the Blynk App at line 19
```cpp
#define AUTH "PASTE_YOUR_TOKEN_HERE" 
```
It will look like this
```cpp
#define AUTH "CMSDB3hzs2xHSaJHgvKLMBhxYneHOMGxysLS"
```
After that open [Blynk website](https://blynk.cloud/dashboard/) and do the Steps as stated:

Click on templates -> Click on your template -> Events ->Edits -> Add new Event

DOOR EVENT
![General Settings](https://github.com/SudoSu-bham/Home_Automation_Security/assets/55135022/3d3fc0e6-124e-4ac5-aac0-8b7a925285e2)
![Notification Settings](https://github.com/SudoSu-bham/Home_Automation_Security/assets/55135022/c5c2d8b5-12e6-4c2f-90f4-db77cb6a8f01)



After doing this Click on save 

SMOKE EVENT
![General Settings](https://github.com/SudoSu-bham/Home_Automation_Security/assets/55135022/fc16b815-11ef-4bc8-be04-28abca496f1f)
![Notification Settings](https://github.com/SudoSu-bham/Home_Automation_Security/assets/55135022/31fd67e6-02ca-42a0-93bc-d2668f6031ee)

When both event created click on Save and Apply

After doing all these processes watch the [video](https://www.youtube.com/) and configure your Blynk mobile application.
https://www.youtube.com/

### Wiring Diagram
![Wiring image](wiring diagram)

![breadboard image](original image)
