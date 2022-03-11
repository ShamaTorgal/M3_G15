# Remote keyless entry (RKE) system
#### Table of Content
     1. Introduction
     2. High Level Requirements
     3. Low Level Requirements

     
## 1. Introduction     
 ![Block Diagram](https://github.com/ShamaTorgal/M3_G15/blob/main/Project1/1_Requirements/RKEsys.webp)
 
Remote keyless entry (RKE) system is a system designed to remotely lock or unlock access to automobiles.

RKE transmission requires two components - a transmitter and a receiver.

• Transmitter - RKE key fob, other ID device with RKE integrated

• Receiver - Body Control ECU, other ECU with integrated RKE

RKE operates by broadcasting radio waves on a particular frequency unidirectionally.

RKE systems implement encryption and rolling code algorithms to prevent car thieves from intercepting and spoofing the telegrams.

## 2. High Level Requirements

|ID	| Description |
| --- | --- |
|HLR_01|	Locking the Car	It shall turn ON all the Led’s on at the same time.|
|HLR_02	|Unlocking the Car	It shall turn OFF all the Led’s on at the same time.|
|HLR_03	|Alarm activation/deactivation	It shall turn On All Led’s in clockwise manner|
|HLR_04	|Approach light	It shall turn OFF All led on in anti-clockwise manner.|

## 3. Low Level Requirements

|ID|	Description|
| --- | --- |
|LLR_01|	Pressing the switch one time	It shall lock the car.|
|LLR_02|	Pressing the switch two times	It shall unlock the car.|
|LLR_03	|Pressing the switch three times	It shall activate/deactivate the Alarm.|
|LLR_04	|Pressing the switch four times	It shall approach the ligh.|
