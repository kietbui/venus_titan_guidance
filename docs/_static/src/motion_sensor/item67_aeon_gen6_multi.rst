Aeotec Z-Wave Plus ZW100 6-in-1 Motion Sensor
--------------------------------

	.. image:: ../../images/motion_sensor/aeon_gen6_motion.jpg
	.. :align: left

Product Description
~~~~~~~~~~~~~~~~~~~~~~~~~~	
	#. 6-in-1 Z-Wave Plus MultiSensor: motion, humidity, temperature, light lux, UV, vibration sensor.
	#. 2 year battery life
	#. Super-small at 1.8 inches. Can be installed in corner, in-wall, on shelf or in downlight.

Working with PhD
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Monitor Aeotec 6-in-1 Motion Sensor and other connected devices with the Zinno app available on iOS&Android
	#. Receive alerts from PhD if the Aeotec 6-in-1 Motion Sensor detects movement
	#. Associate Aeotec 6-in-1 Motion Sensor with other smart devices in Zinno App, and set them to turn on or off when sensor detects movement	

Add Aeotec 6-in-1 Motion Sensor to PhD's network
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. On the Zinno app, press Left Menu Bar, then select “Devices”
	#. Select “+” button to put the PhD in inclusion mode, keep the sensor close to PhD within 10 feet (3 meters)
	#. Press the Action Button on Aeotec 6-in-1 Motion Sensor
	#. If detecting a new device successfully, PhD will announce “Found Device”, and Zinno app will display the dialog box, asking user to interact with device one more time
	#. Repeat step #3, PhD will announce “The device is being added”
	#. If adding the sensor successfully, PhD will announce “Adding Aeotec Sensor Multilevel 6 success” and on Zinno app will display the dialog boxes that indicate user has added device successfully	

	.. image:: ../../images/motion_sensor/aeon_gen6_motion_b.png
	.. :align: center	
	
Specification
~~~~~~~~~~~~~~~~~~~~~~
	- Model number: 				ZW100
	- Power source: 				USB DC 5V, Battery
	- Battery type:					2 CR123A batteries
	- Protocol: 					Z-Wave Plus
	- Dimension:					1.8 x 2.5 x 1.8 inches
	- Weight:						0.13 pounds
	- Color: 						White

	
.. Specification
.. ~~~~~~~~~~~~~~~~~~~~~~
	- Model number: ZW100
	- Power Supply: USB DC 5V or battery power(2×CR123A batteries, 3V, 1500mAh)
	- Operating Temperature: 0 C to 40 C .
	- Measured Temperature Range: -10 C to 50 C . Accuracy: ±0.5 C .
	- Humidity Range: 20%RH to 80%RH. Accuracy: ±5%RH (at 25 C ).
	- Lighting: 0 LUX to 1000 LUX.
	- Motion Sensitivity: 3 meters to 5 meters.
	- Water Proofing: IP20.
	- Wireless Range: Up to 500feet/150 metres outdoors.

.. Inclusion/Exclusion to/from a network
.. ~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Press program button once. Device will be included/excluded to/from zwave network.
	
	.. image:: ../../images/motion_sensor/aeon_gen6_motion_b.png
	.. :align: center
	
.. Wake up information
.. ~~~~~~~~~~~~~~~~~~~~~~~~~
	- When battery is used, to wake up device, press and hold its Z-Wave Button for 3 seconds and then release it. Your MultiSensor’s LED should now be solid to indicate that it is active.
	- When completing configurating or communicating with device, to put device into sleep mode for battery saving, press and hold its Z-Wave Button for 3 seconds and then release it.
	- When power-supply is used, device is in waken up state always.

.. Factory reset
.. ~~~~~~~~~~~~~~~~~
	Press and hold z-wave button for 20 seconds and then release. LED will stay in solid for 2 seconds and then turn off indicates reset successfully.
	
	
.. Button pressed actions and events
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	====================================	===============================================================================
	Short 1 time pressed					1. Send non-secure node info frame
											2. Add device to z-wave network
											3. Remove device from z-wave network
	Short 2 times pressed in 1 seconds		Send secure node info frame
	Press and hold 3 seconds				Enable/disable wake up for 10 minutes
	Press and hold 20 seconds				Reset device to factory setting
	====================================	===============================================================================
	
.. Link in Amazon
.. ~~~~~~~~~~~~~~~~~~
	https://www.amazon.com/Aeotec-Multisensor-temperature-humidity-vibration/dp/B0151Z8ZQY
	
.. Configuration description
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~
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
	
	#. Motion sensity
		- Parameter: 4 (0x04)
		- Size: 1 byte
		- Value: 
			+ 0x00: disable 
			+ 0x01: sensity minimum level 
			+ 0x02: 
			+ 0x03: sensity medium level
			+ 0x04
			+ 0x05: sensity maximum level
		- Default: 5
	
	#. Motion trigger command
		- Parameter: 5 (0x05)
		- Size: 1 byte
		- Value: 
			+ 0x01: Basic set CC 
			+ 0x02: Sensor binary report
		- Default: 1

	#. Configure low battery value
		- Parameter: 39 (0x27)
		- Size: 1 byte
		- Value: 
			+ Valid value: 10 ~ 50
			+ Unit percentage
		- Default: 20

	#. Enable auto report when temperature and humidity change reach to threshold
		- Parameter: 40 (0x28)
		- Size: 1 byte
		- Value: 
			+ 0x00: disable this feature
			+ 0x01: enable this feature
		- Default: 0

	#. Temperature change threshold to send report
		- Parameter: 41 (0x29)
		- Size: 2 bytes
		- Value: 
			+ Unit is Farenheit for US version and Celsius for EU/AU version
			+ High byte is threshold value. low byte is unit (0x01-celsius, 0x02=farenheit)
			+ Threshold value contains 1 decimal point, eg: threshold = 20, it means 2.0. setting value 0x1401 means that 2.0 oC
		- Default: 0x14xx

	#. Humidity change threshold to send report
		- Parameter: 42 (0x2A)
		- Size: 1 byte
		- Value: 
			+ Unit is percentage
			+ Valid value: 0x01 ~ 0x64
		- Default: 0x0A

	#. Luminance change threshold to send report
		- Parameter: 43 (0x2B)
		- Size: 2 bytes
		- Value: in range
		- Default: 0x0064

	#. Battery change
		- Parameter: 44 (0x2C)
		- Size: 1 byte
		- Value: 
			+ Unit is percentage
			+ Valid value: 0x01 ~ 0x64
		- Default: 0x0A

	#. Ultraviolet change
		- Parameter: 45 (0x2D)
		- Size: 1 byte
		- Value: in range
		- Default: 0x02

	#. Low temperature threshold report
		- Parameter: 46 (0x2E)
		- Size: 1 byte
		- Value: 
			+ 0x00: disable
			+ 0x01: enable
		- Default: 0x00

	#. Report items to group 1
		- Parameter: 101 (0x65)
		- Size: 4 bytes
		- Value: bit setting
			+ bit 0: battery
			+ bit 4: ultra-violet
			+ bit 5: temperature
			+ bit 6: humidity
			+ bit 7: luminance
		- Default: 0x000000F1


	#. Auto report interval
		- Parameter: 111 (0x6F)
		- Size: 4 bytes
		- Value: 
			+ Valid value:  0x05-0x28DE80
			+ USB power, unit is second
			+ Battery power: value <= X*60, interval is X minutes
		- Default: 0x00000E10 (3600 seconds)
