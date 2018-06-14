GoControl Z-Wave WAPIRZ-1 PIR Motion Sensor
------------------------------

	.. image:: ../../images/motion_sensor/gocontrol_home_motion.jpg
	.. :align: left

Product Description
~~~~~~~~~~~~~~~~~~~~~~~~~~	
	#. The GoControl Z-Wave Infrared Motion Detector provides motion-based security alerts and can also let you know about temperature changes for the area being surveyed
	#. Its motion detection range is between 6 and 32 feet, and it senses and reports changes in temperature of 2 degrees Fahrenheit or greater, if desired
	
Working with PhD
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Monitor your GoControl Motion Sensor and other connected devices with the Zinno app available on iOS&Android
	#. Receive alerts from PhD if the GoControl Motion Sensor movement
	#. Associate GoControl Motion Sensor with other smart devices in Zinno App, and set them to turn on or off when sensor detects movement, or a change in temperature
	
Add GoControl Motion Sensor to PhD's network
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. On Zinno App, go to Menu → Devices → Tap "+" button to put PhD to inclusion mode
	#. Press program button once. Device will be included/excluded to/from zwave network.
	
	.. image:: ../../images/motion_sensor/gocontrol_home_motion_b.png
	.. :align: left
	

Specification
~~~~~~~~~~~~~~~~~~~~~~
	- Model number: 				WAPIRZ-1
	- Power source: 				Battery
	- Battery type:					CR123A Lithium
	- Protocol: 					Z-Wave
	- Dimension:					1.8 x 2.3 x 3.5 inches
	- Weight:						0.15 pounds
	- Color: 						White
	
.. Specification
.. ~~~~~~~~~~~~~~~~~~~~~~~
	- CR123A Lithium Battery
	- Working frequency: 908.42 MHz
	- Operating temperature: 5°F~140°F / -15°C~ 60°C
	- Up to 100 feet line of sight between the Z-Wave Controller and/or the closest Z-Wave Repeater
	
.. Basic operation
.. ~~~~~~~~~~~~~~~~~~~~~~~
	- During normal operation without detecting any motion, the detector’s red LED will be off.
	- When the sensor detects motion, it will send a status of “ON” (Basic Set,Value: 0xFF) and alarm report (Type: 07, Level: 0xFF) to any associated nodes. The red LED will flash once.
	- When no movement is detected for 3 minutes (adjustable by configuration setting), the detector will send a status of “OFF” (Basic Set, Value: 0x00) and alarm restore report (Type: 07, Level: 0x00) to any associated nodes, then the unit assumes “sleep” mode.
	- The motion detector is equipped with a tamper switch. If the cover of the detector is removed, it will send an alarm report (Type: 07, Level: 0xFF) and the red LED will light constant.


.. Inclusion/Exclusion to/from a network
.. ~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Press program button once. Device will be included/excluded to/from zwave network.
	
	.. image:: ../../images/motion_sensor/gocontrol_home_motion_b.png
	.. :align: left
	
.. Link in Amazon
.. ~~~~~~~~~~~~~~~~~
	https://www.amazon.com/GoControl-Z-Wave-PIR-Motion-Detector/dp/B00MOF3EU2
	
.. Configuration description
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Re-trigger Wait Time
		- Parameter: 1 (0x01)
		- Size: 2 bytes
		- Value: 
			+ valid value: 0x0000 ~ 0x00FF
			+ Unit is minute
		- Default: 0x0003

