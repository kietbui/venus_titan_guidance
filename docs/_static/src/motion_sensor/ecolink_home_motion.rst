Ecolink Z-Wave PIRZWAVE1 Motion Sensor
--------------------------------

	.. image:: ../../images/motion_sensor/ecolink_home_motion.jpg
	.. :align: left

Product Description
~~~~~~~~~~~~~~~~~~~~~~~~~~	
	#. 33 or 55 lb. pet immune 
	#. 90-degree look down 
	#. Tamper protected
..	#. 5-8 year battery life on 1 CR123A lithium battery
	
Working with PhD
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Monitor your Ecolink Motion Sensor and other connected devices with the Zinno app available on iOS&Android
	#. Receive alerts from PhD if the Ecolink Motion Sensor detects movement
	#. Associate Ecolink Motion Sensor with other smart devices in Zinno App, and set them to turn on or off when sensor detects movement
	
Add Ecolink Motion Sensor to PhD's network
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. On the Zinno app, press Left Menu Bar, then select “Devices”
	#. Select “+” button to put the PhD in inclusion mode, keep the sensor close to PhD within 10 feet (3 meters)
	#. If detecting a new device successfully, PhD will announce “Found Device”, and Zinno app will display the dialog box, asking user to interact with device one more time
	#. Repeat step #3, PhD will announce “The device is being added”
	#. If adding the sensor successfully, PhD will announce “Adding Ecolink Motion Sensor success” and on Zinno app will display the dialog boxes that indicate user has added device successfully
	
	.. image:: ../../images/motion_sensor/ecolink_motion_sensor_i.jpg
	.. image:: ../../images/motion_sensor/ecolink_motion_sensor_b.png
	.. :align: left

Specification
~~~~~~~~~~~~~~~~~~~~~~
	- Model number: 				PIRZWAVE1
	- Power source: 				Battery
	- Battery type:					x1 CR123A Lithium
	- Protocol: 					Z-Wave
	- Dimension:					1.8 x 2.3 x 3.5 inches
	- Weight:						0.15 pounds
	- Color: 						White
	
	
.. Specification
.. ~~~~~~~~~~~~~~~~~~~~~~~~~
	- Operating frequency: 908.42 MHz
	- Operating range: up to 100 feet (30.5meters) line of sign
	- Operating temperature: 0-49 oC (32-120 oF)
	- Detection radius: 39 feet
	- Detection angle: 45 degrees
	- Battery: 3V lithium CR123A
	- Battery life: approxiately 3 years

.. Inclusion/Exclusion to/from a network
.. ~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Press program button once. Device will be included/excluded to/from zwave network.
	
	
	.. image:: ../../images/motion_sensor/ecolink_motion_sensor_i.jpg
	.. image:: ../../images/motion_sensor/ecolink_motion_sensor_b.png
	.. :align: left

.. Jumper setting
.. ~~~~~~~~~~~~~~~~~~
	.. image:: ../../images/motion_sensor/home_motion_jumper.png
	.. :align: left
	
.. Link in Amazon
.. ~~~~~~~~~~~~~~~~
	https://www.amazon.com/Ecolink-Z-Wave-Motion-Detector-PIRZWAVE2-ECO/dp/B00FB1TBKS

.. Configuration description
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Trigger OFF to associated device
		- Parameter: 99 (0x63)
		- Size: 1 byte
		- Value: 
			+ 0x00: disable
			+ 0x01: enable
		- Default: 0x01
