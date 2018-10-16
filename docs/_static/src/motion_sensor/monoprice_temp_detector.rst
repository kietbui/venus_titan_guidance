Monoprice Z-Wave Plus 15374 Motion Sensor
-----------------------------------

	.. image:: ../../images/motion_sensor/monoprice_temp_detector.jpg
	.. :align: left
	
Product Description
~~~~~~~~~~~~~~~~~~~~~~~~~~	
	#. Easy to Install
	#. Low Power
	#. Motion Detection: This device uses a passive infrared sensor and sends a Z-Wave Plus® signal when motion is detected within its detection range
	#. Can detect moving objects within line of sight at distances up to 32 feet, away with a field of view up to 120°
	#. This sensor detects changes in temperature and reports the temperature to the network whenever a significant change has occurred
	
Working with PhD
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Monitor your Monoprice Motion Sensor and other connected devices with the Zinno app available on iOS&Android
	#. Receive alerts from PhD if the Monoprice Motion Sensor detects movement
	#. Associate Monoprice Motion Sensor with other smart devices in Zinno App, and set them to turn on or off when sensor detects movement, or a change in temperature
	
Add Monoprice Motion Sensor to PhD's network
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. On Zinno App, go to Menu → Devices → Tap "+" button to put PhD to inclusion mode
	#. Press program button once. Device will be included/excluded to/from zwave network.
		
	.. image:: ../../images/motion_sensor/monoprice_motion_with_temp_d.png
	.. :align: left
	

Specification
~~~~~~~~~~~~~~~~~~~~~~
	- Model number: 				15374
	- Power source: 				Battery
	- Battery type:					CR123A Lithium
	- Protocol: 					Z-Wave
	- Dimension:					1.8 x 2.3 x 3.5 inches
	- Weight:						0.15 pounds
	- Color: 						White

.. Basic operation
.. ~~~~~~~~~~~~~~~~~~~~~~~
	- Walking in front of the sensor sends an ON status signal (Basic set, value 0xFF) to any associated nodes. The led flashes once when this occurs.
	- After an ON status signal is sent, the sensor will monitor the area for additional motion. If no motion is detected wthin about 3 seconds, it will send an OFF status signal (Basic set, value 0x00)
	- LED is off during normal operation
	- The sensor is equipped with tamper switch.
	
.. Specification
.. ~~~~~~~~~~~~~~~~~~~~~~~
	- Operating frequency: 908.42 MHz
	- Operating range: Up to 100 feet line of sign
	- Opeating temperature: 5 ~ 140 oF (-15 ~ 60 oC)
	- Battery: 1xCR123A 
	
.. Inclusion/Exclusion to/from a network
.. ~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Press program button once. Device will be included/excluded to/from zwave network.
		
	.. image:: ../../images/motion_sensor/monoprice_motion_with_temp_d.png
	.. :align: left

.. Link in Amazon
.. ~~~~~~~~~~~~~~~~~~~~~~~
	https://www.amazon.com/Monoprice-Z-Wave-Motion-Detector-Temperature/dp/B01I5YETV8
	
.. Configuration description
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~
	There is no configuration for this device.
