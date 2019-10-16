#                                                 Group AK Project Progress Report 
#                                                                         -- Waking-up System for Rear Window Defogger

## Current Progress


1.Tested the functionality of required devices(DS18B20 Temperature Sensor, DHT11 Temperature & Humidity Sensor)

The group have tested the two sensors by measuring our living environment temperature and relative humidity and showing the data into python.


2.Determined the formulas for further exploitation of collected data. Figured out how to align the relative humidity acquired by the T&H sensor. 

The group have found a way to align the relative humidity acquired from the T&H sensor by not using the humidity value directly but combining it with another temperature value collected on the surface of “window”. In this way, the group acquire a more accurate relative humidity value to monitor and keep it below 90%. The formulas and steps for processing data are shown as following:

input T1 RH1  # values collected from T&H sensor

return d1=f(T1,RH1)  

input T2   # values from T sensor

return RH2=f(T2,d1)

3. Set up reasonable expectations for the final “waking-up” system

As expected, the final finished product for in-class demonstration should be a glass box with two sensors and a buzzer alarm attached. However, due to the restriction that low temperature and high humidity are not conventional, the group need to record a video in advance showing how this system works in the required environment (low temperature as in the refrigerator, high humidity as additional water vapor injection). 

## Problems Encountered

1. Build up an applicable simulation system with low temperature and high humidity;

First, the group need to get a legit glass box. Then, just as mentioned in the group's vision for the final system, the restriction of unconventional surroundings makes it harder to show and build up. So the group may need to adjust the settings of the refrigerator to meet their needs. Finally, although the group have tested the functionality for each sensor, the availability of the whole system cannot be assured only if the system has been built up. 
 
2. Processing collected data using Python

The code is complicated and need to be well designed for gathering targeted data and control the whole system. 

The humidity sensor is not sensitive enough to detect the slight change of relative humidity. Only dramatic change in humidity can activate the function of the whole system. 

The temperature sensor may not be closely attached to the window, so that the temperature change on window may not be accurate enough to predict the formation of fog. 

## Future Plan

1. Write a python code 

Since the group raised the idea of building up a calculation model, the next step is to define a suitable function in Python to acquire final relative humidity set by using collected data. Although mathematical model is easy to be understood, accurately appling this model to Python still needs to be considered.

2. Set up the experiment model for testing the performance of our sensor system, which will include a glass box, refrigerator, sensors and buzzer

Determine an appropriate experiment model to test the performance of this sensor system is important. Two of the most crucial factors when doing test are temperature and humidity. 
