Ecolink Door Window Sensor
--------------------------------
Ecolink Intelligent Technology Z-Wave Easy Install, Battery Operated, Door/Window Sensor, White & Brown (DWZWAVE2-ECO)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

	.. image:: ../../images/door_sensor/ecolink_door_window.jpg
	.. :align: left

Specification
~~~~~~~~~~~~~~~~~~~~~
	- Z-Wave enabled device which provides open/closed position status
	- Transmits open/closed status
	- Report tamper condition when cover is open
	- For in-door use only
	- Operating in 908.42 MHz
	- Range: up to 100 feet line-of-sight
	- Operating temperature: 32 - 120 Fareinheit
	- Battery: 3V CR123A
	- Battery life approximately 3 years

Inclusion/Exclusion to/from a network
~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Remove battery then re-install battery to reset. Device will be included/excluded to/from zwave network.
	
Wake up information
~~~~~~~~~~~~~~~~~~~~~
	- By default, a sensor is configured to send Wake Up Notification frames every three hours.
	
Link in Amazon
~~~~~~~~~~~~~~~~~
	https://www.amazon.com/Ecolink-Intelligent-Technology-Operated-DWZWAVE2-ECO/dp/B00HPIYJWU/
	
Configuration description
~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Parameter 99: Send basic set 0x00 to associated devices when door sensor door is closed
		- Parameter: 99 (0x63)
		- Size: 1 byte
		- Value:
			(1) 0 = disable feature
			(2) 1 = enable feature
		- Default: 0
