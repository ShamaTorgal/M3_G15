# Remote keyless entry (RKE) system
#### Table of Content
     1. Introduction
     2. Requirements
         1.1 High Level Requirements
         1.2 Low Level Requirements
     3. SWOT
     4. 5W's 1H

     
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

## 3. S.W.O.T

![WhatsApp Image 2022-03-11 at 11 40 39](https://github.com/ShamaTorgal/M3_G15/blob/main/1.RKE/1_Requirements/1.jpg)

## 4. 5W's 1H
 ![Block Diagram](https://github.com/ShamaTorgal/M3_G15/blob/main/1.RKE/1_Requirements/5W1H.png)

* WHO- People who have vehicle.
* WHAT- It is a system which wirelessly lock/unlock door of a vehicle and perform different functionalities from a distance.
* WHEN- Whenever the user wants to lock or unlock the door of the vehicle and wants to use its other features.
* WHERE- It can be use anywhere
* WHY- For an easy use of vehicle and to ensure secuirity.
* HOW- The system can be operated by just clicking a button .

