# BiCom System
#### Table of Content
     1. Introduction
     2. Requirements
          2.1 High Level Requirements
          2.2 Low Level Requirements
          2.3 Features
     3. SWOT
     4. 4W's 1H
     5. Architecture
     6. Test plan 
         6.1 High level Test Plan
         6.2 Low level Test Plan

## 1. Introduction

 ![Block Diagram](https://github.com/ShamaTorgal/M3_G15/blob/main/2.BiCom/1_Requirements/Bicomsys.jpg)
 
* A BiCom system is the extention of the unidirectional RKE(Remote Keyless Entry) to bidirectional RKE system.
* It displays various features like window status,alarm status,car battery info and door status.
* It is basically a communication between the keyfob and car.
* LEDs are used for signalling like if the blue switch is pressed all LEDs are ON at the same time which prints the window status of the car.

## 2. Requirements

### 2.1 High Level Requirements

|ID	|	Description|
| --- | --- |
|HLR_01|	Print window status	-It shall turn ON all Leds at the same time.|
|HLR_02	|Print alarm status	-It shall turn OFF all Leds at the same time.|
|HLR_03	|Print car battery info	-It shall turn ON  Leds  in clock wise manner.|
|HLR_04	|Print Door status	-It shall turn ON Leds in anti clockwise manner.|


### 2.2 Low Level Requirements

|ID|	Description|
| --- | --- |
|LLR_01|	Pressing switch One time	-It shall print the window status|
|LLR_02|	Pressing switch two time	-It shall print the alarm status.|
|LLR_03	|Pressing the switch three time -It shall print the car battery info.|
|LLR_04	|Pressing the switch four times -It shall print the door status.|

### 2.3 Features
* Use to lock or unlock vehicles from a distance.
* Small in size and handy too.
* Have approach light functionality.
* Keeps the vehicle secure.
* Can activate/deactivate alarm of the vehicle
* Have LEDs to indicate which functionality is currently performing.

## 3. S.W.O.T

![WhatsApp Image 2022-03-11 at 12 16 44](https://user-images.githubusercontent.com/98829310/157816983-06f5fef0-7dae-4118-9cb7-feddf844a05f.jpeg)

## 4. 5W's 1H

 ![Block Diagram](https://github.com/ShamaTorgal/M3_G15/blob/main/2.BiCom/1_Requirements/5w1h.jpg)
 
* WHO- People who have vehicle.
* WHAT- It is a system which wirelessly lock/unlock door of a vehicle and perform different functionalities from a distance.
* WHEN- Whenever the user wants to lock or unlock the door of the vehicle and wants to use its other features.
* WHERE- It can be use anywhere
* WHY- For an easy use of vehicle and to ensure secuirity.
* HOW- The system can be operated by just clicking a button.

## 5. Architecture

![Block Diagram](https://github.com/ShamaTorgal/M3_G15/blob/main/2.BiCom/2_Architecture/image3.jpg)

![Block Diagram](https://github.com/ShamaTorgal/M3_G15/blob/main/2.BiCom/2_Architecture/image4.jpg)

![Block Diagram](https://github.com/ShamaTorgal/M3_G15/blob/main/2.BiCom/2_Architecture/image5.jpg)


## 6. Test Plan

### 6.1 HIGH LEVEL TEST PLAN

|TestID|	Description	| exp Input| exp	Output|	Status|
| --- | --- | --- | --- | --- |
|HL01	|Encryption|	Only authorized key can access the Car control|	Authorized key required to access the Car control	|Passing|
|HL02	|Remote |Car Locking	switch pressed 1 times|	Car Locked	|Passing|
|HL03	|Remote |Car unlocking	switch pressed 2 times|	Car unlocked	|Passing|
|HL04	|Alram |Activation	switch pressed 3 time	|Alarm Activated	|Passing|
|HL05	|Alram |Deactivation	switch pressed 3 times|	Alarm deactivated	|Passing|
|HL06	|Approach |Light	switch pressed 4 times	|Approch Light Turned ON |	Passing|

### 6.2 LOW LEVEL TEST PLAN

|TestID|	Description	| exp Input	| exp Output|	Status|
| --- | --- | --- | --- | --- |
|LL01|	All LEDs Should get turn ON together when Car is locked	|switch pressed 1 times|	All Leds are ON	|Passing|
|LL02	|All LEDs Should get turn OFF together when Car is unlocked	|switch pressed 2 times|	All Leds are OFF	|Passing|
|LL03	|Alram Activation	|switch pressed 3 time|	LEDs turned ON one by one in clockwise direction	|Passing|
|LL04	|Alram deactivation	|switch pressed 3 time|	LEDs turned OFF one by one in clockwise direction	|Passing|
|LL05	|Approach light	|switch pressed 4 time|	LEDs turned ON one by one in anticlockwise direction	|Passing|
