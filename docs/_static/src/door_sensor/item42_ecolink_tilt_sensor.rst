Ecolink Z-Wave TILTZWAVE2-ECO Garage Door Tilt Sensor
--------------------------------

	.. image:: ../../images/door_sensor/ecolink_tilt_sensor.jpg
	.. :align: left

Product Description
~~~~~~~~~~~~~~~~~~~~~~
	#. Easy installs with included flush mount bracket and begins to learn as soon as batteries power it up. 
	#. Five year battery life and discrete design keep it out of sight and out of mind when not on alert. 
	#. External contact input available for external triggers.

Working with PhD
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Be monitored by PhD via the Zinno app available on iOS&Android
	#. Associate Ecolink Tilt Sensor with other smart devices in Zinno App, and set them turn on or off if the sensor detects that the garage door has been opened or left open
	
Add Ecolink Tilt Sensor to PhD's network
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. On Zinno App, go to Menu → Devices → Tap "+" button to put PhD to inclusion mode
	#. Remove battery then re-install battery to reset. Device will be included/excluded to/from zwave network.
	
	.. image:: ../../images/door_sensor/ecolink_tilt_sensor_i.jpg
	.. :align: left
	
Specification
~~~~~~~~~~~~~~~~~~~~~~
	- Model number: 				TILTZWAVE2-ECO
	- Power source: 				Battery
	- Protocol: 					Z-Wave
	- Battery type: 				CR123A Lithium
	- Dimension:					1.7 x 3.3 x 4.1 inches
	- Weight:						0.1 lb
	- Color: 						White

.. Inclusion/Exclusion to/from a network
.. ~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Remove battery then re-install battery to reset. Device will be included/excluded to/from zwave network.
	
	.. image:: ../../images/door_sensor/ecolink_tilt_sensor_i.jpg
	.. :align: left
	
.. Link in Amazon
.. ~~~~~~~~~~~~~~~~~~~
	https://www.amazon.com/Ecolink-Z-Wave-Wireless-Tilt-Sensor/dp/B00HGVJRX2/
	
.. Configuration description
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Parameter 99: Send basic set 0x00 to associated devices when door sensor door is closed
		- Parameter: 99 (0x63)
		- Size: 1 byte
		- Value:
			(1) 0 = disable feature
			(2) 1 = enable feature
		- Default: 0
