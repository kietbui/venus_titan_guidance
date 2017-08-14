Schlage Home Motion Sensor
--------------------------------
Schlage Z-Wave Home Motion Sensor with Nexia Home Intelligence, RS200 , Cert ID: ZC08-12030002 by Schlage Lock Company
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

	.. image:: ../../images/motion_sensor/schlage_home_motion.jpg
	.. :align: left

Specification
~~~~~~~~~~~~~~~~~~~~~
	- For indoor use only
	- 90° wide angle detection pattern
	- Operating frequency: 908.42 MHz
	- Operation range: Up to 100 feet (30.5 meters) line-of-sight
	- Operating temperature: 0° – 49°C, 32° – 120°F
	- Battery type required: 3V Lithium CR123A
	- Battery life approximately 3 years

Inclusion/Exclusion to/from a network
~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Press program button once. Device will be included/excluded to/from zwave network.
		
	.. image:: ../../images/motion_sensor/schlage_home_motion_b.png
	.. :align: left

Jumper setting
~~~~~~~~~~~~~~~~~~
	.. image:: ../../images/motion_sensor/home_motion_jumper.png
	.. :align: left

Link in Amazon
~~~~~~~~~~~~~~~~~~~~
	https://www.amazon.com/Schlage-Z-Wave-Motion-Sensor-Intelligence/dp/B018A1P7XK
	
Configuration description
~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Trigger OFF to associated device
		- Parameter: 99 (0x63)
		- Size: 1 byte
		- Value: 
			+ 0x00: disable
			+ 0x01: enable
		- Default: 0x01

