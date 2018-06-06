Aeon Labs  Z-Wave DSB29-ZWUS Door/Window Sensor, 2nd Edition
--------------------------------

	.. image:: ../../images/door_sensor/aeon_door_window.jpg
	.. :align: left

Product Description
~~~~~~~~~~~~~~~~~~~
	#. Signal up to 6 associated Z-Wave devices when contact is broken
	#. 300 foot communicating Z-Wave RF range
	#. Long 2 year battery life
	#. Tamper prevention security trigger
	#. DIY installation with double stick tape or screws

Working with PhD
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Be monitored by PhD via the Zinno app available on iOS&Android
	#. The Speaker on Phd will annouce when receive the alert from the Aeon Door/Window Sensor
	#. Associate Aeon Door/Window Sensor with other smart devices in Zinno App, and set them turn on or off if the sensor detects doors or windows have been open

Add Aeon Door/Window Sensor to PhD's network
~~~~~~~~~~~~~~~~~~~~~~~
	#. On Zinno App, go to Menu → Devices → Tap "+" button to put PhD to inclusion mode
	#. Press the Action button once
	#. Wait for PhD completes inclusion/exclusion process
	
	.. image:: ../../images/door_sensor/aeon_door_window_d.jpg
	.. :align: left

Specification
~~~~~~~~~~~~~~~~~~~~~~
	- Model number: 				DSB29-ZWUS
	- Power source: 				Battery
	- Protocol: 					Z-Wave
	- Battery type: 				2xAAA 
	- Dimension:					2.9 x 0.8 x 1.1 inches
	- Weight:						0.13 lb
	- Color: 						White
	
.. Wake up information
.. ~~~~~~~~~~~~~~~~~~~~~
	- D/W sensor will keep wake up for 8 seconds after it send wake up notification command. 
	- If it receive a command,it will keep wake up for 8 seconds to wait next command.
	- Press tamper switch 3 times, then D/W sensor will wake 10 minutes.
	- If configured, d/w sensor will wake 10 minutes too when power on.
	- Only 3 ways can abort this status:
		- Pressing tamper switch 3 times, sleep right now;
		- D/W sensor received “Wake up no more information CC”, sleep right now;
		- Received other command, wake 8 seconds to wait next command.

.. LED indicator
.. ~~~~~~~~~~~~~~~~~~
	- ON: In network
	- OFF: Sleeping
	- Blink: Out of network

.. Button actions
.. ~~~~~~~~~~~~~~~~~~
	#. Press Action button once: 
		1. Send node info frame without security CC in node info list.
		2. Put device to Inclusion/Exclusion mode
	#. Press Action button twice with 1 second:
		1. Send node info frame with security CC in node info list.
		2. Put device to Inclusion/Exclusion mode
	#. Press and hold the Action Button for 3 seconds and then released
		Toggle on/off 10 minutes wake-up state
	#. Press and hold Action bitton for 20 seconds then release:
		Reset Door Window Sensor to Factory Default
		

.. Configuration description
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~

	#. Parameter 1: To set which value of the Sensor Binary Report will be sent when the door is Opened/Closed.
		- Paramter: 1 (0x01)
		- Size: 1 byte
		- Value: 
			1, Value=0, Close=Sensor Binary Report 0xFF,Open=Sensor Binary Report 0x00.
			2, Value=1, Close= Sensor Binary Report 0x00, Open=Sensor Binary Report 0xFF.
		- Default: 1
	
	#. Parameter 2: Enable/disable wake-up 10 minutes when re-power on the Sensor. 
		- Paramter: 2 (0x02)
		- Size: 1 byte
		- Value: 0=disable, 1=enable
		- Default: 1
		
	#. Parameter 3: To set which value of the Basic Set will be sent when the door is Opened/Closed.
		- Paramter: 3 (0x03)
		- Size: 1 byte
		- Value: 
			1, Value=0, Close= Basic Set 0xFF, Open=Basic Set 0x00.
			2, Value=1, Close=Basic Set 0x00, Open= Basic Set 0xFF.
		- Default: 1
		
	#. Parameter 39: Set the low battery value.
		- Paramter: 39 (0x27)
		- Size: 1 byte
		- Value: from 10% to 50% 
		- Default: 10
		
	#. Parameter 111: Set the interval time of battery report.
		- Paramter: 111 (0x6F)
		- Size: 4 byte
		- Value: 
			Value = 0: disable battery report for an interval time
			Value=1 to 0x7FFFFFFF, the interval time of battery report.
			Note:
				1, if the value is less than 10, the time unit is second. If the value is more than 10, the time unit is 4 minutes, which means if the value is more than 10 and less than 240, the interval time is 4 minutes. If the value is more than 240 and less than 480, the interval is 8 minutes. 2, if the current battery report falls below the low battery value (configurable parameter 39), it will send battery report=0xFF.
		- Default: 0

	#. Parameter 121: To configure which sensor report will be sent when the Sensor is triggered On/Off.
		- Paramter: 121 (0x79)
		- Size: 1 byte
		- Value: Bit setting
			1. Bit 8: Basic set
			2. Bit 4: Sensor binary report
			3. Others: reserved
		- Default: 0x00000100

