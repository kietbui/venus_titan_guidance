Ecolink Tilt Sensor
--------------------------------
Ecolink Intelligent Technology Z-Wave Garage Door Tilt Sensor, White (TILT-ZWAVE2-ECO)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


	.. image:: ../../images/door_sensor/ecolink_tilt_sensor.jpg
	.. :align: left

Overview
~~~~~~~~~~~~~~~~~~~~~~
	- Z-Wave enabled devices which transmits when a garage door is opened or closed
	- Use a tilt sensor to detect the angle of a door and transmit open/closed status
	- Reports tamoer condition if cover is removed
	
Specification
~~~~~~~~~~~~~~~~~~~~~~
	
	- In-door use only
	- Operating frequency: 908.42 MHz
	- Range: Up to 100 feet line-of-size
	- Operating temperature: 32 - 120 Fareinheit
	- Battery type: 3V Lithium CR123A

Inclusion/Exclusion to/from a network
~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Remove battery then re-install battery to reset. Device will be included/excluded to/from zwave network.
	
	.. image:: ../../images/door_sensor/ecolink_tilt_sensor_i.jpg
	.. :align: left
	
Link in Amazon
~~~~~~~~~~~~~~~~~~~
	https://www.amazon.com/Ecolink-Intelligent-Technology-Z-Wave-TILT-ZWAVE2-ECO/dp/B00HGVJRX2
	
Configuration description
~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Parameter 99: Send basic set 0x00 to associated devices when door sensor door is closed
		- Parameter: 99 (0x63)
		- Size: 1 byte
		- Value:
			(1) 0 = disable feature
			(2) 1 = enable feature
		- Default: 0
