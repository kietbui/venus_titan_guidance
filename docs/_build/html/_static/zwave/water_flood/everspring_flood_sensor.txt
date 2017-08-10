Everspring Water/Flood Sensor
-------------------------------
Everspring Z-Wave Water/Flood Sensor
~~~~~~~~~~~~~~~~~~~~~~~~~~~

	.. image:: ../../images/water_flood/everspring_flood_sensor.jpg
	.. :align: left
	
Brief information
~~~~~~~~~~~~~~~~~~~~~~~~
	

Specification
~~~~~~~~~~~~~~~~~~~~~~~~
	- Battery: 1.5V AAx3 pieces
	- Battery life: about 1 year, @25oC standby mode
	- Operating frequency: 868.42MHz (ST812-1) / 908.42MHz (ST812-2) 

Inclusion/Exclusion to/from a network
~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Press program button 3 times within 1.5 seconds and wait for exclusion completes
	#. Press program button 3 times within 1.5 seconds again and wait for inclusion completes


	.. image:: ../../images/water_flood/everspring_flood_sensor_b.png
	.. :align: left

Factory reset
~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Press program button 3 times within 1.5 seconds
	#. Within 1 second, press and hold program button until beep tone stops
	#. LED is ON 2 seconds then OFF 2 seconds until completing process


Configuration description
~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Basic set level
		- Parameter: 1 (0x01)
		- Size: 1 byte
		- Value:
			+ 0x00: OFF
			+ 0x01 ~ 0x63: ON for ON/OFF devices and dim level for dimmable devices
		- Default: 0x63
		
