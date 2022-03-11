# Test Plan

## HIGH LEVEL TEST PLAN

|TestID|	Description	| exp Input| exp	Output|	Status|
| --- | --- | --- | --- | --- |
|HL01	|Encryption|	Only authorized key can access the Car control|	Authorized key required to access the Car control	|Passing|
|HL02	|Remote |Car Locking	switch pressed 1 times|	Car Locked	|Passing|
|HL03	|Remote |Car unlocking	switch pressed 2 times|	Car unlocked	|Passing|
|HL04	|Alram |Activation	switch pressed 3 time	|Alarm Activated	|Passing|
|HL05	|Alram |Deactivation	switch pressed 3 times|	Alarm deactivated	|Passing|
|HL06	|Approach |Light	switch pressed 4 times	|Approch Light Turned ON |	Passing|

## LOW LEVEL TEST PLAN

|TestID|	Description	| exp Input	| exp Output|	Status|
| --- | --- | --- | --- | --- |
|LL01|	All LEDs Should get turn ON together when Car is locked	|switch pressed 1 times|	All Leds are ON	|Passing|
|LL02	|All LEDs Should get turn OFF together when Car is unlocked	|switch pressed 2 times|	All Leds are OFF	|Passing|
|LL03	|Alram Activation	|switch pressed 3 time|	LEDs turned ON one by one in clockwise direction	|Passing|
|LL04	|Alram deactivation	|switch pressed 3 time|	LEDs turned OFF one by one in clockwise direction	|Passing|
|LL05	|Approach light	|switch pressed 4 time|	LEDs turned ON one by one in anticlockwise direction	|Passing|
