Schlage Z-Wave BE468CAM619 Touchscreen Deadbolt Smart Lock
----------------------------------------

	.. image:: ../../images/door_lock/schlage_connect_camelot_be468.jpg
	.. :align: left
	
Product Description
~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Durable Resistive Touchscreen with matte finish to protect against fingerprints and smudges
	#. Anti-pick shield protects against lock tampering
	#. ED backlight for easy keypad access in the dark;do not use a power drill for installation  
	#. Available in a range of colors.
	
Working with PhD
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Control your Schlage Smart Lock and other connected devices with the Zinno app available on iOS&Android
	#. With PhD, you could automatically set it open when you arrive home or close when you leave
	#. Associate Schlage Smart Lock with other smart devices in Zinno App, and set them to turn on or off when you lock or unlock your Schlage Smart Lock

Add Schlage Smart Lock to PhD's network
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. On Zinno App, go to Menu → Devices → "+" button to put PhD to inclusion mode
	#. While PhD is in searching mode, bring the lock close, then enter 6-digit programing code then press '0' and wait for inclusion completes
		
	.. image:: ../../images/door_lock/schlage_connect_camelot_touchscreen_d.png
	.. :align: left
	
Specification
~~~~~~~~~~~~~~~~~~~~~~
	- Model number: 				BE468CAM619
	- Power source: 				Battery
	- Protocol: 					Z-Wave
	- Battery type: 				4xAA 
	- Dimension:					4.5 x 9.2 x 5.1 inches
	- Weight:					3.8 pounds
	- Color: 	Aged Bronze, Bright Brass, Bright Chrome, Satin Chrome, Satin Chrome
	
Others
~~~~~~~~~~~~~~~~~~~~~~~~
	.. image:: ../../images/door_lock/schlage_connect_camelot_be468_prg_1.jpg
	.. :align: left
	
	.. image:: ../../images/door_lock/schlage_connect_camelot_be468_prg_2.jpg
	.. :align: left
	
	.. image:: ../../images/door_lock/schlage_connect_camelot_be468_prg_3.jpg
	.. :align: left
.. Brief information
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~
	- Thumbturn: Used to lock and unlock manually from the inside.
	- Schlage Button: 
		+ Located on the outside of the door.
		+ Press to exit programming mode immediately.
		+ The first button you will press when entering a user and in the programming process.
	- Touchscreen: 
		+ Located on the outside of the door.
		+ Used to enter codes for programming and unlocking.
		+ Remains unlit until the Schlage button is pressed.
	- Cylinder: Used to unlock only in emergency situations
	- Bolt: 
		+ Automatically extends and retracts when the touchscreen is used
		+ Manually extends and retracts when the thumbturn is rotated
	
	.. image:: ../../images/door_lock/schlage_connect_camelot_be468_prg_1.jpg
	.. :align: left
	
	.. image:: ../../images/door_lock/schlage_connect_camelot_be468_prg_2.jpg
	.. :align: left
	
	.. image:: ../../images/door_lock/schlage_connect_camelot_be468_prg_3.jpg
	.. :align: left

.. Inclusion/Exclusion to/from a network
.. ~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Input programing code then press '0' and wait for exclusion completes
	#. Input programing code then press '0' again and wait for inclusion completes
		
	.. image:: ../../images/door_lock/schlage_connect_camelot_touchscreen_d.png
	.. :align: left

.. Configuration description
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~
	
	#. Enable beeper
		- Parameter: 3 (0x03)
		- Size: 1 byte
		- Value: 
			0x00: Disable feature
			0xFF: Enable feature
		- Default: 0x00
	
	#. Enable vacation mode
		- Parameter: 4 (0x04)
		- Size: 1 byte
		- Value: 
			0x00: Disable feature
			0xFF: Enable feature
		- Default: 0x00
	
	#. Enable lock & leave
		- Parameter: 5 (0x05)
		- Size: 1 byte
		- Value: 
			0x00: Disable feature
			0xFF: Enable feature
		- Default: 0x00

	#. Auto lock
		- Parameter: 15 (0x0F)
		- Size: 1 byte
		- Value: 
			0x00: Disable feature
			0xFF: Enable feature
		- Default: 0xFF

	#. User pin code length
		- Parameter: 16 (0x10)
		- Size: 1 byte
		- Value: 0x04 – 0x08 
		- Default: 0x04

