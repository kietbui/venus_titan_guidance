Ecolink Home Motion Sensor
--------------------------------
Ecolink Z-Wave PIR Motion Detector, Pet Immune (PIRZWAVE2-ECO)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

	.. image:: ../../images/motion_sensor/ecolink_home_motion.jpg
	.. :align: left


Specification
~~~~~~~~~~~~~~~~~~~~~~~~~
	- Operating frequency: 908.42 MHz
	- Operating range: up to 100 feet (30.5meters) line of sign
	- Operating temperature: 0-49 oC (32-120 oF)
	- Detection radius: 39 feet
	- Detection angle: 45 degrees
	- Battery: 3V lithium CR123A
	- Battery life: approxiately 3 years

Inclusion/Exclusion to/from a network
~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Press program button once and wait for exclusion completes
	#. Press program button once again and wait for inclusion completes
	
	
	.. image:: ../../images/motion_sensor/ecolink_motion_sensor_i.jpg
	.. image:: ../../images/motion_sensor/ecolink_motion_sensor_b.png
	.. :align: left

Jumper setting
~~~~~~~~~~~~~~~~~~
	.. image:: ../../images/motion_sensor/home_motion_jumper.png
	.. :align: left
	

Configuration description
~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Trigger OFF to associated device
		- Parameter: 99 (0x63)
		- Size: 1 byte
		- Value: 
			+ 0x00: disable
			+ 0x01: enable
		- Default: 0x01
