Ecolink Z-Wave DWZWAVE2-ECO Door/Window Sensor
--------------------------------

	.. image:: ../../images/door_sensor/ecolink_door_window.jpg
	.. :align: left

Product Description
~~~~~~~~~~~~~~~~~~~
	#. Features industry leading Rare Earth Magnets that allow for up to a 5/8 inch gap , which makes it perfect for double hung or commercial windows.
	#. Easy installation by simply pulling the battery tab to begin the learning process.
	#. Both white and brown plastic casing included to match any décor.

Working with PhD
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Be monitored by PhD via the Zinno app available on iOS&Android
	#. The Speaker on Phd will annouce when receive the alert from the Ecolink Door/Window Sensor
	#. Associate Ecolink Door/Window Sensor with other smart devices in Zinno App, and set them turn on or off if the sensor detects doors or windows have been open	

Add Ecolink Door/Window Sensor to PhD's network
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. On Zinno App, go to Menu → Devices → Tap "+" button to put PhD to inclusion mode
	#. Remove battery then re-install battery to reset. Device will be included/excluded to/from zwave network.
	
Specification
~~~~~~~~~~~~~~~~~~~~~~
	- Model number: 				DWZWAVE2-ECO
	- Power source: 				Battery
	- Protocol: 					Z-Wave
	- Battery type: 				CR123A 
	- Dimension:					3.4 x 1 x 1 inches
	- Weight:						0.2 lb
	- Color: 						White & Brown

	
.. Specification
.. ~~~~~~~~~~~~~~~~~~~~~
	- Z-Wave enabled device which provides open/closed position status
	- Transmits open/closed status
	- Report tamper condition when cover is open
	- For in-door use only
	- Operating in 908.42 MHz
	- Range: up to 100 feet line-of-sight
	- Operating temperature: 32 - 120 Fareinheit
	- Battery: 3V CR123A
	- Battery life approximately 3 years

.. Inclusion/Exclusion to/from a network
.. ~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Remove battery then re-install battery to reset. Device will be included/excluded to/from zwave network.
	
.. Wake up information
.. ~~~~~~~~~~~~~~~~~~~~~
	- By default, a sensor is configured to send Wake Up Notification frames every three hours.
	
.. Link in Amazon
.. ~~~~~~~~~~~~~~~~~
	https://www.amazon.com/Ecolink-Intelligent-Technology-Operated-DWZWAVE2-ECO/dp/B00HPIYJWU/
	
.. Configuration description
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Parameter 99: Send basic set 0x00 to associated devices when door sensor door is closed
		- Parameter: 99 (0x63)
		- Size: 1 byte
		- Value:
			(1) 0 = disable feature
			(2) 1 = enable feature
		- Default: 0
