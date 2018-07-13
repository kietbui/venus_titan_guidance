EverSpring Z-Wave ST814-2 Multi Sensor
--------------------------------

	.. image:: ../../images/multi_sensor/everspring_temp_humi_detector.jpg
	.. :align: left
	
Product Description
~~~~~~~~~~~~~~~~~~~~~~~~~~	
	#. Z-Wave compatible temperature / humidity sensor.
	#. Includes LCD display with Fahrenheit and Celcius temps.
	#. Give warnings when temperature or humidity reaches preset trigger values.
	
Working with PhD
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Monitor temperature or humidity from EverSpring Multi Sensor 	
	
Add EverSpring Multi Sensor to PhD's network
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. On the Zinno app, press Left Menu Bar, then select “Devices”
	#. Select “+” button to put the PhD in inclusion mode, keep the sensor close to PhD within 10 feet (3 meters)
	#. Press Temperature unit button 3 times within 1.5 seconds
	#. If detecting a new device successfully, PhD will announce “Found Device”, and Zinno app will display the dialog box, asking user to interact with device one more time
	#. Repeat step #3, PhD will announce “The device is being added”
	#. If adding the sensor successfully, PhD will announce “Adding Everspring Temperature Humidity Sensor success” and on Zinno app will display the dialog boxes that indicate user has added device successfully

	.. image:: ../../images/multi_sensor/everspring_temp_humi_detector_d.jpg
	.. :align: left	

Specification
~~~~~~~~~~~~~~~~~~~~~~
	- Model number: 				ST814-2
	- Power source: 				USB DC 5V, Battery
	- Battery type:					x3 AA batteries
	- Protocol: 					Z-Wave
	- Dimension:					3.8 x 3.5 x 2.8 inches
	- Weight:						0.5 pounds
	- Color: 						White

	
.. Specification
.. ~~~~~~~~~~~~~~~~~~~~~~
	- Operating freq: 868.42MHz (ST814-1) / 908.42MHz (ST814-2)
	- Operating temp: -10℃ ~ 50℃
	- Relative humidity range: 20% ~ 90% 
	- Temperature unit: Celsius/Farenheit
	- Battery: 3x1.5V-AAA
	- Operating range: Up to 30m line of sign


.. Inclusion/Exclusion to/from a network
.. ~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Presses Temperature unit button 3 times within 1.5seconds. Device will be included/excluded to/from zwave network.
	
	.. image:: ../../images/multi_sensor/everspring_temp_humi_detector_d.jpg
	.. :align: left
	
.. Link in Amazon
.. ~~~~~~~~~~~~~~~~~~~~~
	https://www.amazon.com/Everspring-Z-Wave-Temperature-Humidity-ST814-2/dp/B00RYWBBU0
	
.. Configuration description
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Basic set level: set level to associated devices
		- Parameter: 1 (0x01)
		- Size: 1 byte
		- Value:
			+ 0x00: Disable
			+ 0x01 - 0x63: dim level
		- Default:
			+ Default set: 0x63
			+ Factory default: 0x63
	
	#. Temperature trigger ON value
		- Parameter: 2 (0x02)
		- Size: 1 byte
		- Value:
			+ 0x94 - 0x32: temperature trigger ON
			+ 0x63: clear temperature trigger ON
			+ unit is degree
		- Default:
			+ Default set: 0x1E
			+ Factory default: 0x63
	
	#.Temperature trigger OFF value
		- Parameter: 3 (0x03)
		- Size: 1 byte
		- Value:
			+ 0x94 - 0x32: temperature trigger OFF
			+ 0x63: clear temperature trigger OFF
			+ unit is degree
		- Default:
			+ Default set: 0x14
			+ Factory default: 0x63
	
	#. Humidity trigger ON value
		- Parameter: 4 (0x04)
		- Size: 1 byte
		- Value:
			+ 0x0D - 0x5A: humidity trigger ON
			+ 0x63: clear humidity trigger ON
			+ unit is percentage
		- Default:
			+ Default set: 0x32
			+ Factory default: 0x63
		
	#. Humidity trigger OFF value
		- Parameter: 5 (0x05)
		- Size: 1 byte
		- Value:
			+ 0x0D - 0x5A: humidity trigger OFF
			+ 0x63: clear humidity trigger OFF
			+ unit is percentage
		- Default:
			+ Default set: 0x28
			+ Factory default: 0x63
	
	#. Auto report interval
		- Parameter: 6 (0x06)
		- Size: 2 bytes
		- Value:
			+ 0x0000: disable
			+ 0x0001 - 0x059F: set minutes
		- Default:
			+ Default set: 0x0000
			+ Factory default: 0x0000
		
	#. Temperature change report threshold
		- Parameter: 7 (0x07)
		- Size: 1 byte
		- Value:
			+ 0x01 - 0x46: temperature change threshold
			+ 0x00: disable
			+ unit is degree
		- Default:
			+ Default set: 0x00
			+ Factory default: 0x00
	
	#. Humidity change report threshold
		- Parameter: 8 (0x08)
		- Size: 1 byte
		- Value:
			+ 0x05 - 0x46: humidity change threshold
			+ 0x00: disable
			+ unit is percentage
		- Default:
			+ Default set: 0x00
			+ Factory default: 0x00
	
