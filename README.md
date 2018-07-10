<img align="right" src="images/led.gif">
# LED Controller
A simple tutorial on how to control an LED using Dialog IoT Platform

## Get your gear
* NodeMCU
* Micro USB cable
* LED
* 330Ω resistor
* Male-female jumper wires
* Breadboard

<p align="center">
  <img width="500" src="/images/components.PNG">
</p>


### Create your developer account at https://portal.iot.ideamart.io

  * Once you have completed the registration process, Please click the email confirmation link which is sent to your registered email address & then contact one of our ideamart admins to activate your account.
  * After the approval, login to your account and follow the steps below
  
1. Create your device configuration in the developer portal
   1. Click on **Device Onboarding(json)** under **Device Management**
   1. Select **Generic_brand_xxx** under **Device Definitions**
    1. Choose MQTT from the dropdown menu under **Connection Method** & click **Save**
  
<p align="center">
  <img width="700" src="/images/DeviceConf.png">
</p>

    1. Click **Add Action** under **Action** create **ON**,**OFF** actions as below & then click **Save**
  
<p align="center">
  <img width="700" src="/images/on.PNG">
</p>

<p align="center">
  <img width="700" src="/images/off.PNG">
</p>  

1. Now go to **Device Operation** under **Device Management** and click **Add Device**
 1. Enter the required parameters as follows and click **Save**
 
<p align="center">
  <img width="350" src="/images/SaveDevice.png">
</p>  

 1. Once sucessfully saved, your new device will be visible under the **Devices** tab as shown below 
 
<p align="center">
  <img width="700" src="/images/DeviceSaved.png">
</p>  

### Let's modify the device firmware(Arduino Code) according to your device properties
 * Download the **LED_Controller.zip** and extract it to your preferred location
 * Open the **.ino** file inside the folder named **LED_Controller**
 * The code has 3 differnt parts namely **LED_controller, main, your_actions_events**. You have to modify only the **LED_Controller** to sucessfully control your **LED**
 * Please change the values of **BRAND,TYPE,VERSION,MAC_ADDRESS** under **Device Details** to your device's properties
 
 
 * Also change the **username** & **password** under **WiFi Credentials** to your own WiFi username & password (Home router/Mobile hotspot)
 
 
 ## Connect your circuit as shown below
<p align="center">
  <img width="500" src="/images/circuit_diagram.png">
</p>

