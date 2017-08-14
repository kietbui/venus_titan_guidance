Monoprice motion sensor
---------------------------------
Monoprice Z-Wave Motion Detector with Temperature Sensor, NO LOGO by Monoprice
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

	.. image:: ../../images/motion_sensor/monoprice_temp_detector.jpg
	.. :align: left
	

Basic operation
~~~~~~~~~~~~~~~~~~~~~~~
	- Walking in front of the sensor sends an ON status signal (Basic set, value 0xFF) to any associated nodes. The led flashes once when this occurs.
	- After an ON status signal is sent, the sensor will monitor the area for additional motion. If no motion is detected wthin about 3 seconds, it will send an OFF status signal (Basic set, value 0x00)
	- LED is off during normal operation
	- The sensor is equipped with tamper switch.
	
Specification
~~~~~~~~~~~~~~~~~~~~~~~
	- Operating frequency: 908.42 MHz
	- Operating range: Up to 100 feet line of sign
	- Opeating temperature: 5 ~ 140 oF (-15 ~ 60 oC)
	- Battery: 1xCR123A 
	
Inclusion/Exclusion to/from a network
~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Press program button once. Device will be included/excluded to/from zwave network.
		
	.. image:: ../../images/motion_sensor/monoprice_motion_with_temp_d.png
	.. :align: left

Link in Amazon
~~~~~~~~~~~~~~~~~~~~~~~
	https://www.amazon.com/Monoprice-Z-Wave-Motion-Detector-Temperature/dp/B01I5YETV8
	
Configuration description
~~~~~~~~~~~~~~~~~~~~~~~~~~
	There is no configuration for this device.
