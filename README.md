# STM32Fxx
Programs on STM32 Discovery kit


Unzip files to open the project directly in keil.

Mems_accerlometer Project:
Accelerometer_mems sensor in board is tested by blinking corresponding led based on board movement.
when User button is pressed then led's will toggle.

Mems_critical Project.

It has
Three Threads 
1) Mems sensor LED blink.
2) All Led's switches on for 2 sec and then switches off.
3) Two led's switches on for 2 sec and then switches off.

Led's is shared resource here for threads.
So Led's are protected using mutex's.

Thread which grabs the mutex will be executed,other threads will wait till mutex is released.
Once,Mems sensor thread starts,it will keep on executing until user button is pressed.


Threads execution in Event viewer ans system viewer.



