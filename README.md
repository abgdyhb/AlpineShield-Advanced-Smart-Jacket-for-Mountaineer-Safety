# 🏔️ Alpine Shield Smart Jacket Project

A **smart wearable safety system** designed for mountaineers to monitor vital health parameters and environmental conditions in real-time.  
This project combines **IoT, sensor integration, GPS, and wireless communication** into a modular wearable jacket that enhances safety and decision-making during expeditions.  

---

## 📖 Introduction
Mountaineering exposes climbers to extreme environments with risks such as **altitude sickness, hypothermia, frostbite, rapid weather changes, avalanches, and toxic gases**.  
In remote areas, lack of immediate medical assistance and reliable communication often leads to undetected fatalities.  

The **Alpine Shiels Project** offers a compact safety solution by integrating:
- Real-time health monitoring (heart rate, oxygen, body temperature, muscle activity)  
- Environmental tracking (temperature, humidity, air pressure, wind speed, rainfall)  
- Wireless data transmission and GPS tracking  

This system ensures proactive decision-making, quick emergency response, and improved climber survival.  

---

## 🎯 Objectives
- **Health Monitoring**: Enable mountaineers to track vital health parameters such as heart rate, blood pressure, body temperature, and muscle activity in real-time.  
- **Environmental Awareness**: Integrate sensors to monitor fluctuations in temperature, humidity, air pressure, wind speed, and rainfall.  
- **Connectivity & Safety**: Provide real-time GPS tracking and wireless communication using NRF modules for emergency assistance.  
- **Modular Design**: Deliver a **wearable jacket system** with detachable compartments for easy maintenance and organization of components.  
- **Decision Support**: Improve overall safety, performance, and decision-making by combining health and environmental data into a single, user-friendly platform.  

---


## 📖 Result and Discussions

The microcontroller controls all the health monitoring
Sensors and sends the data to the caretaker through the
NRF module. A buzzer is there for an emergency signal
to send the signal to the caretaker in case if any health
emergency occurs.
The data monitored by the system includes the heart rate,
body and atmospheric temperature, pulse rate,
atmospheric and body pressure, and real time location of
the climber, ensuring a through tracking system. This
system is vital in extreme conditions where health and
location data need to be transmitted continuously for the
climber’s safety.

## A. Health Monitoring
The real time results recorded display the climber’s body temperature, heart rate, atmospheric pressure, and oxygen saturation (SpO2). For instance, at 19:33:22, the body temperature reads 69.00°F,heart rate 114.07 BPM, body pressure 130.00 hPa, and SpO2 98.00. These values are sent regularly to the Telegram bot, for
the constant communication of the climber’s condition to the base station as well as the caretaker in case of emergencies.

## B. Telegram Bot Messages for Health Monitoring
The Telegram bot, named “Mountain Saver” receives and records the climber’s health parameters at continuous
intervals. The values are almost similar to those shown in the serial monitor which confirms the successful data
transmission from the microcontroller. The variations in body pressure exhibit the system’s ability to track real time health fluctuations. 

## C. ECG Result
The ECG module tracks the climber’s heart activity, with electrodes attached at specific points on the body. 

## D. EMG Waveforms
The EMG sensor captures muscle activity, explicitly contraction and relaxation, essential for monitoring physical
exertion. The health data and real time location are relayed to the caretaker and base camp through the NRF module, ensuring assistance in the event of an emergency. The graph shows two conditions: resting and working. During resting periods, the EMG reading is relatively the same which indicates stable conditions in the first graph. However, during physical exertion like climbing or muscle activity, the second graph shows corresponding spikes.

## E. Weather Monitoring
Atmospheric pressure fluctuates from 332.82 hPa to 714.25 hPa, indicating significant changes in weather conditions or elevation. Temperature readings range between 27.80°C and 29.40°C. Humidity levels vary from 47% to 52%. The altitude readings show a broad range, from 2053.94 meters to 8063.21 meters, likely due to changes in mountain altitudes.

## F. Emergency Message
Based on the defined thresholds, the health monitoring system must evaluate. When limits are exceeded by these values an automatic alert is transmitted to rescue personnel. Racks in our device contain an activation button which sends quick alerts to rescue teams when climbers experience illness.

## G. GPS Navigation
The serial monitor captures the system’s connection to Wi-Fi and its response to threshold violations. When the sensor detects environmental conditions that exceed a preset threshold, triggering an emergency alert, displaying the message: “Threshold value exceed, Emergency!!!” This function is designed to detect critical conditions, indicating risks for mountain climbers. The emergency alert is configured to send the notification to the Telegram bot, informing the user, caretaker and base camp in real time, which enhances safety during expedition. 

## VI. CONCLUSION
The proposed prototype will help the climber and as well as safeguard of the mountaineers to track the health condition of the climber along with the real time data transmission system has proven potential to decrease mortality rates through live monitoring by safeguards who inspect health records alongside geographical position and atmospheric information. The safeguards in the base can
track the health and real time location of the mountaineers along with the environmental condition of the mountains. The current NRF module in the system holds a major limitation because its wireless communication range proves insufficient when operating in mountainous environments. The LoRa module demonstrates superior performance in distance coverage and environmental efficiency, so it seems like a better wireless communication choice for this purpose.
The jacket should integrate camera technology to generate live video feedback that will help rescue teams during operations. The system transforms into a dependable security companion for mountaineers through these upgrades which enables better response together with
improved preparedness during emergency situations.




