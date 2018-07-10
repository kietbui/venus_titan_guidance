Schlage Z-Wave RS200 Motion Sensor
--------------------------------

	.. image:: ../../images/motion_sensor/schlage_home_motion.jpg
	.. :align: left

Product Description
~~~~~~~~~~~~~~~~~~~~~~~~~~	
	#. For indoor use only
	#. 90° wide angle detection pattern
	#. Operating frequency: 908.42 MHz
	#. Operation range: Up to 100 feet (30.5 meters) line-of-sight
	#. Operating temperature: 0° – 49°C, 32° – 120°F

Working with PhD
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Monitor your Schlage Motion Sensor and other connected devices with the Zinno app available on iOS&Android
	#. Receive alerts from PhD if the Schlage Motion Sensor detects movement
	#. Associate Schlage Motion Sensor with other smart devices in Zinno App, and set them to turn on or off when sensor detects movement

Add NYCE Curtain Motion Sensor to PhD's network
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. On the Zinno app, press Left Menu Bar, then select “Devices”
	#. Select “+” button to put the PhD in inclusion mode
	#. Use a pin or paper clip to press the program button on the back of the Sensor case
	#. If detecting a new device successfully, PhD will announce “Found Device”, and Zinno app will display the dialog box, asking user to interact with device one more time
	#. Repeat step #3, PhD will announce “The device is being added”
	#. If adding the sensor successfully, PhD will announce “Adding Schlage Motion Sensor success” and on Zinno app will display the dialog boxes that indicate user has added device successfully
		
	.. image:: ../../images/motion_sensor/schlage_home_motion_b.png
	.. :align: left

Specification
~~~~~~~~~~~~~~~~~~~~~~
	- Model number: 				RS200
	- Power source: 				Battery
	- Battery type:					CR123A Lithium
	- Protocol: 					Z-Wave
	- Dimension:					3.5 x 2.5 x 2 inches
	- Weight:						0.21 pounds
	- Color: 						White	
	
Jumper setting
~~~~~~~~~~~~~~~~~~
	.. image:: ../../images/motion_sensor/home_motion_jumper.png
	.. :align: left

.. Link in Amazon
.. ~~~~~~~~~~~~~~~~~~~~
	https://www.amazon.com/Schlage-Z-Wave-Motion-Sensor-Intelligence/dp/B018A1P7XK
	
.. Configuration description
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Trigger OFF to associated device
		- Parameter: 99 (0x63)
		- Size: 1 byte
		- Value: 
			+ 0x00: disable
			+ 0x01: enable
		- Default: 0x01

