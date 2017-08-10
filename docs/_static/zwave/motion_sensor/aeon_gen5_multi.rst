Aeon Labs Gen5 Multi-Sensor
--------------------------------
Aeon Labs Aeotec Z-Wave Multi-Sensor
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

	.. image:: ../../images/motion_sensor/aeon_gen5_motion.jpg
	.. :align: left

Specification
~~~~~~~~~~~~~~~~~~~~~~~~~
	- Power Supply: USB DC 5V or battery power(4×AAA batteries)
	- Operating Temperature: -10 oC to 60 oC .
	- Measured Temperature Range: -10 C to 50 C . Accuracy: ±1 oC .
	- Humidity Range: 20% to 80%. Accuracy: ±5% (at 25 oC ).
	- Lighting: 0 LUX to 1000 LUX.
	- Motion Sensitivity: 3 meters to 5 meters.
	- Water Proofing: IP42
	- Wireless Range: Up to 600feet/150 metres outdoors.

Inclusion/Exclusion to/from a network
~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Press program button once and wait for exclusion completes
	#. Press program button once again and wait for inclusion completes
	
	
	.. image:: ../../images/motion_sensor/aeon_gen5_motion_b.jpg
	.. :align: center
	
Wake up information
~~~~~~~~~~~~~~~~~~~~~~~~~
	- When battery is used, to wake up device, press and hold its Z-Wave Button for 3 seconds and then release it. Your MultiSensor’s LED should now be solid to indicate that it is active.
	- When completing configurating or communicating with device, to put device into sleep mode for battery saving, press and hold its Z-Wave Button for 3 seconds and then release it.
	- When power-supply is used, device is in waken up state always.
	
Factory reset
~~~~~~~~~~~~~~~~~
	Press and hold z-wave button for 20 seconds and then release. LED will stay in solid for 2 seconds and then turn off indicates reset successfully.
	
Button pressed actions and events
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	====================================	===============================================================================
	Short 1 time pressed					Add device to z-wave network
											Remove device from z-wave network
	Press and hold 3 seconds				Send Wake Up Notification (when it is in battery power)
	Press and hold 20 seconds				Reset device to factory setting
	====================================	===============================================================================
	

Configuration description
~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Enable wake-up device 10 minutes after re-power on (battery mode)
		- Parameter: 2 (0x02)
		- Size: 1 byte
		- Value: 
			0x00: disable
			others: enable
		- Default: 0x00

	#. Auto clear motion interval
		- Parameter: 3 (0x03)
		- Size: 2 bytes
		- Value: 1 ~ 15300
			+ 1 ~ 255: unit is second
			+ 256 ~ 15300: unit is minute with below formular
				a. interval = value/60 (without remainder)
				b. interval = value/60 + 1 (if remainder)
		- Default: 0x00F0
	
	#. Enable motion sensor
		- Parameter: 4 (0x04)
		- Size: 1 byte
		- Value: 
			+ 0x00: disable
			+ 0x01: enable
		- Default: 1
	
	#. Trigger commands for motion sensor
		- Parameter: 5 (0x05)
		- Size: 1 byte
		- Value: 
			+ 0x01: basic set CC (for associated devices)
			+ 0x02: sensor binary report CC (for controller)
		- Default: 1
	
	#. Enable report when measurements reach certain threshold or percentage
		- Parameter: 40 (0x28)
		- Size: 1 byte
		- Value: 
			+ 0x00: diable
			+ 0x01: enable
		- Default: 0

	#. Temperature change threshold
		- Parameter: 41 (0x29)
		- Size: 2 bytes
		- Value: 
			a. when unit is Celcius, threshold = set value
			b. when unit is Farenheit, threshold = set value * 1.8
			c. High byte is part of integer, low byte is the fractional part
		- Default: 0x0100
			
	#. Huminity change
		- Parameter: 42 (0x2A)
		- Size: 2 bytes
		- Value:
			+ Unit is percentage
			+ High byte is part of integer, low byte is the fractional part
		- Default: 0x0500

	#. Luminance change
		- Parameter: 43 (0x2B)
		- Size: 2 bytes
		- Value:
			+ Unit is LUX
			+ High byte is part of integer, low byte is the fractional part
		- Default: 0x6400 (100 LUX)
	
	#. Battery change
		- Parameter: 44 (0x2C)
		- Size: 2 bytes
		- Value:
			+ Unit is percentage
			+ High byte is part of integer, low byte is the fractional part
		- Default: 0x0500 (100 LUX)
			
	#. Low temperature report
		When this feature is enabled, sensor will report 0xFFFF to controller in case current temperature is lower than -15oC
		- Parameter: 46 (0x2E)
		- Size: 1 byte
		- Value:
			+ 0x00: disable this feature
			+ 0x01: enable this feature
		- Default: 0x00
	
	#. Report items to group 1
		- Parameter: 101 (0x65)
		- Size: 4 bytes
		- Value: 0x05~0x28DE80
			+ bit 0: battery
			+ bit 5: temperature
			+ bit 6: Humidity
			+ bit 7: luminance
		- Default: 0x000000E1 (all above items are selected)

	#. Auto report interval to group 1
		- Parameter: 111 (0x6F)
		- Size: 1 byte
		- Value:
			+ Unit is second
			+ Valid value: 0x05~0x28DE80
		- Default: 0x00000708
