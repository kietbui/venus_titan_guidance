Schlage Home Door Window Sensor
--------------------------------
Z-Wave Door and Window Sensor with Nexia, RS 100, Both White and Brown Cases Included
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

	.. image:: ../../images/door_window/schlage_door_window.jpg
	.. :align: left

Overvirew
~~~~~~~~~~~~~~~~~~~~~
- Z-Wave enabled device which provides open/closed position status
	- Transmits open/closed status
	- Report tamper when cover is open

Specification
~~~~~~~~~~~~~~~~~~~~~
	- For indoor use only
	- Operating frequency: 908.42 MHz
	- Operation range: Up to 100 feet (30.5 meters) line-of-sight
	- Operating temperature: 0° – 49°C, 32° – 120°F (ambient temperature)
	- Battery type required: 3V Lithium CR123A
	- Battery life approximately 3 years
	
Inclusion/Exclusion to/from a network
~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Remove battery then re-install battery to reset
	#. Remove battery for at least 5 seconds then re-insert to add
	#. Wait for controller completes inclusion/exclusion process
		
	.. image:: ../../images/door_window/ecolink_door_window_i.jpg
	.. :align: left
	
LED indicator
~~~~~~~~~~~~~~~~~~~
	- Continuously blinking: device is not in any z-wave network
	- Solid light: device is in a z-wave network or tamper
	- Single blink: Open/Close detected
	

Configuration description
~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Parameter 99: Send basic set 0x00 to associated devices when door sensor door is closed
		- Parameter: 99 (0x63)
		- Size: 1 byte
		- Value:
			(1) 0 = disable feature
			(2) 1 = enable feature
		- Default: 0
