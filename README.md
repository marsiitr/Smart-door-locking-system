# Smart-door-locking-system

#### Open Project 2022

## Abstract 

The aim of this project is to open a Smart door lock from any where in the world by using IOT cloud or by using Keypad. The goals of this project was to build a modern, easy-to-use, smart door lock that allows for accessible unlocking and adds convenience, utility, and security to your home.

## Motivation

Ever felt lazy to go and open the door when you listen to door bell? Or tired of carrying keys all over and afraid of loosing them ?. To provide an easy and convenient method for unlocking a door by removing the need for the old-fashioned key. And the time that is requires to open the door using IOT is less than time required to open with normal key. And it also ensure more security for our lock. 

## Mechanical Aspect of the Design

The actuator used in this project s a 12V Solenoid Lock Actuator. It is a ready-made lock like desin which just as to be fitted in the casing. A case for this has to be made. This need to be done on Solidworks and get it 3D printed. The casing has to be as compact as possible and must fit the PCB, actuator ,etc. Due to time constraints it has not been made.

## Electronics Aspect of the Design

### Components

* Nodemcu ESP 8266 - ESP 8266 : This is used as Wi Fi module to connect the door lock through IoT. It is used to connect to Arduino IoT cloud and send the data from Cloud to Arduino (or vice versa).
* Arduino UNO - This is used to control the door lock and take input through keypad and act on the lock. This is main controlling unit of lock.
* Solenoid Lock Actuator - Linear solenoids basically consist of an electrical coil wound around a cylindrical tube with a ferro magnetic actuator or “plunger” that is free to move or slide “IN” and “OUT” of the coils body. They are useful in many applications that require an open or closed (in or out) type motion. In this case it moves IN when power is supplied and is in OUT state when there’s no power.
* Keypad - Keypad : This is to use ‘password’ based unlocking. Who wants to take out mobile if one is at the door!? We’ve used 4*4 keypad.
* 5V Single relay module
* 12V rechargeable Li-ion Battery
* 12V Charger
* Some diodes, Resistors, Connecting wires
* PCB designing

<p><img width="674" alt="Final ckt" src="https://user-images.githubusercontent.com/109852675/180622980-73ec9dae-7ab8-48cd-b12d-f95311ac56dc.png"></p>

### Working 

First of all, a request to open door lock is sent from Arduino IoT cloud Dashboard. The request is then sent to Nodemcu ESP 8266 via internet. For this Nodemcu must be connected to Wi Fi with internet. Nodemcu then transfers the request to open the door to Arduino UNO by serial communication through Rx and Tx pins. Arduino UNO on the basis of request opens or closes the lock. The door lock automatically closes after 10 seconds of opening.

<p><img width="727" alt="Workflow" src="https://user-images.githubusercontent.com/109852675/180622842-15ab47f4-2f1a-4038-b57d-8b78ae5e9c49.png"></p>


## Cost Structure

	Solenoid Actuator: 500/-
	Arduino Uno: 500/-
	NodeMCU ESP8266: 350/-
	Other costs (Adapters, batteries etc): 700/-

## Applications

* This project has various applications in daily life. Now a days people are too busy and they want to make an advantage of resources in various aspects.
* If you are having only one key to a house then the main problem here is other person of the house may not have the keys, so by using this IOT cloud  many people can access the door lock.
* Disabled or elder people can easily access the door using their mobile phones.And it also ensures high security to the lock.

## Limitations

* The main problem here is if both battery and charging management got failed. Then it is difficult to open the lock. 
* Also Hackers can hack the access to get into the house. We need to keep extra access for Guests, during that period our code can be shared to other people.
* Reliance on Smart Phones. If we lost our mobile and if we dont have any back up option, then we may fall into trouble.
* It Costs Heavily and if some problem occurs we need to contact for help.

## Furter Improvements

* The circuit could be made compact by PCB printing. Also the casing can be done by printing the solid work model.
* LCD Display can be used to show the status of password, lock and other stuff.
* IOT code can be upgraded to store time of door opening in th cloud.
* The Lock can be integrated mechanically with modern door handle.

## Team Members

	1. [Manmanth Ashtikar](https://github.com/ashtikarmanmath)
	2. [Varanasi Chakradhar](https://github.com/Chakri2507)

## Mentor

1. Nishant Kumar
