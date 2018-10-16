Schlage Z-Wave RS100HC Door/Window Sensor
----------------------------------------

	.. image:: ../../images/door_sensor/schlage_door_window.jpg
	.. :align: left

Product Description
~~~~~~~~~~~~~~~~~~~~~~
	#. Simple installation and set up–just stick on
	#. Incorporate into automations so the lights turn on where there is activity
	#. Check in to see if the doors and windows are closed at night
	#. Chose white or brown covers included in each package

Working with PhD
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Be monitored by PhD via the Zinno app available on iOS&Android
	#. The Speaker on Phd will annouce when receive the alert from the Schlage Door/Window Sensor
	#. Associate Schlage Door/Window Sensor with other smart devices in Zinno App, and set them turn on or off if the sensor detects doors or windows have been open	

Add Schlage Door/Window Sensor to PhD's network
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. On Zinno App, go to Menu → Devices → Tap "+" button to put PhD to inclusion mode
	#. Remove battery then re-install battery to reset. Device will be included/excluded to/from zwave network.
		
	.. image:: ../../images/door_sensor/schlage_door_window_detail1.jpg
	.. :align: left
	
Specification
~~~~~~~~~~~~~~~~~~~~~
	- Model number: 				RS100HC
	- Power source: 				Battery
	- Protocol: 					Z-Wave
	- Battery type: 				CR123A
	- Dimension:					3.5 x 1.75 x 1 inches
	- Weight:						0.2 lbs
	- Color: 						White
	
.. Inclusion/Exclusion to/from a network
.. ~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Remove battery then re-install battery to reset. Device will be included/excluded to/from zwave network.
		
	.. image:: ../../images/door_sensor/schlage_door_window_detail1.jpg
	.. :align: left
	
.. LED indicator
.. ~~~~~~~~~~~~~~~~~~~
	- Continuously blinking: device is not in any z-wave network
	- Solid light: device is in a z-wave network or tamper
	- Single blink: Open/Close detected
	
.. Link in Amazon
.. ~~~~~~~~~~~~~~~~~
	https://www.amazon.com/Z-Wave-Window-Sensor-Nexia-Included/dp/B008Q5CTBE

.. Configuration description
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Parameter 99: Send basic set 0x00 to associated devices when door sensor door is closed
		- Parameter: 99 (0x63)
		- Size: 1 byte
		- Value:
			(1) 0 = disable feature
			(2) 1 = enable feature
		- Default: 0
