# Remote keyless entry (RKE) system
#### Table of Content
     1. Introduction
     2. Requirements
         2.1 High Level Requirements
         2.2 Low Level Requirements
     3. SWOT
     4. 5W's 1H
     5. Architecture
     6. Test Plan
         6.1 HIGH LEVEL TEST PLAN
         6.2 LOW LEVEL TEST PLAN
     
## 1. Introduction     
 ![Block Diagram](https://github.com/ShamaTorgal/M3_G15/blob/main/1.RKE/1_Requirements/RKEsys.webp)
 
Remote keyless entry (RKE) systems allow a user to lock and unlock the car using a transmitter on the keychain, which transmits data to a receiver in the vehicle. Remote keyless entry (RKE) system is a system designed to remotely lock or unlock access to automobiles. This system represent the standard solution for conveniently locking and unlocking a vehicle's doors and luggage compartment by remote control. The anti-theft and immobilizer systems can also be turned on and off in this way.

RKE transmission requires two components - a transmitter and a receiver.

• Transmitter - RKE key fob, other ID device with RKE integrated

• Receiver - Body Control ECU, other ECU with integrated RKE

RKE operates by broadcasting radio waves on a particular frequency unidirectionally.

RKE systems implement encryption and rolling code algorithms to prevent car thieves from intercepting and spoofing the telegrams.

## 2. Requirements

### 2.1 High Level Requirements

|ID	| Description |
| --- | --- |
|HLR_01|	Locking the Car	-It shall turn ON all the Led’s on at the same time.|
|HLR_02	|Unlocking the Car	-It shall turn OFF all the Led’s on at the same time.|
|HLR_03	|Alarm activation/deactivation	-It shall turn On All Led’s in clockwise manner|
|HLR_04	|Approach light	-It shall turn OFF All led on in anti-clockwise manner.|

### 2.2 Low Level Requirements

|ID|	Description|
| --- | --- |
|LLR_01|	Pressing the switch one time	-It shall lock the car.|
|LLR_02|	Pressing the switch two times	-It shall unlock the car.|
|LLR_03	|Pressing the switch three times	-It shall activate/deactivate the Alarm.|
|LLR_04	|Pressing the switch four times	-It shall approach the ligh.|

### 2.3 Features
* Use to lock or unlock vehicles from a distance.
* Small in size and handy too.
* Have approach light functionality.
* Keeps the vehicle secure.
* Can activate/deactivate alarm of the vehicle
* Have LEDs to indicate which functionality is currently performing.

## 3. S.W.O.T

![WhatsApp Image 2022-03-11 at 11 40 39](https://github.com/ShamaTorgal/M3_G15/blob/main/1.RKE/1_Requirements/5W1H.png)

## 4. 4W's 1H

 ![Block Diagram](https://github.com/ShamaTorgal/M3_G15/blob/main/1.RKE/1_Requirements/5W1H.png)

* WHO- People who have vehicle.
* WHAT- It is a system which wirelessly lock/unlock door of a vehicle and perform different functionalities from a distance.
* WHEN- Whenever the user wants to lock or unlock the door of the vehicle and wants to use its other features.
* WHERE- It can be use anywhere
* WHY- For an easy use of vehicle and to ensure secuirity.
* HOW- The system can be operated by just clicking a button .

# 5. Architecture

 ![Block Diagram](https://github.com/ShamaTorgal/M3_G15/blob/main/Project1/2_Architecture/image1.jpg)
 
 ![Block Diagram](https://github.com/ShamaTorgal/M3_G15/blob/main/Project1/2_Architecture/image2.jpg)

## 6. TestPlanAndOutput

### 6.1 HIGH LEVEL TEST PLAN
|TestID	|Description	|exp Input	|exp Output| 	Status|
| --- | --- | --- | --- | --- |
|HL01	|Encryption	|Only authorized key can access the Car control	|Authorized key required to access the Car control|	Passing|
|HL02	|Remote Car Locking	|switch pressed 1 times	|Car Locked	|Passing|
|HL03	|Remote Car unlocking	|switch pressed 2 times|	Car unlocked	|Passing|
|HL04	|Alram Activation	|switch pressed 3 time	|Alarm Activated|	Passing|
|HL05	|Alram deactivation	|switch pressed 3 times|	Alarm deactivated|	Passing|
|HL06	|Approach Light	|switch pressed 4 times	|Approch Light Turned ON	|Passing|

### 6.2 LOW LEVEL TEST PLAN

|TestID |	Description | exp	Input | exp	Output|Status|
| --- | --- | --- | --- | --- |
|LL01	|All LEDs Should get turn ON together when Car is locked|	switch pressed 1 times|	All Leds are ON	|Passing|
|LL02	|All LEDs Should get turn OFF together when Car is unlocked	|switch pressed 2 times|	All Leds are OFF|	Passing|
|LL03	|Alram Activation|	switch pressed 3 time	|LEDs turned ON one by one in clockwise direction	|Passing|
|LL04	|Alram deactivation	|switch pressed 3 time|	LEDs turned OFF one by one in clockwise direction	|Passing|
|LL05	|Approach light|	switch pressed 4 time	|LEDs turned ON one by one in anticlockwise direction	|Passing|

