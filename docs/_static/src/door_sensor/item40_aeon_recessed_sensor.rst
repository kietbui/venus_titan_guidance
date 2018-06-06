Aeotec Z-Wave Plus ZW089 Recessed Door/Window Sensor, 2nd Edition
--------------------------------
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

	.. image:: ../../images/door_sensor/aeon_recessed.jpg
	.. :align: left

Product Description
~~~~~~~~~~~~~~~~~~~
	#. Z-Wave security sensor designed to monitor when doors or opened or closed.
	#. Invisibly installed within door / door frame.
	#. Battery powered. Lasts 1 year. Battery included.
	#. Z-Wave Plus certified

Working with PhD
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Be monitored by PhD via the Zinno app available on iOS&Android
	#. The Speaker on Phd will annouce when receive the alert from the Aeotec Recessed Door/Window Sensor
	#. Associate Aeotec Recessed Door/Window Sensor with other smart devices in Zinno App, and set them turn on or off if the sensor detects doors or windows have been open	
	
Add Aeotec Recessed Door/Window Sensor to PhD's network
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. On Zinno App, go to Menu → Devices → Tap "+" button to put PhD to inclusion mode
	#. Press the z-wave button which is hiden under the hole on top of device once. Device will be included/excluded to/from zwave network.

	.. image:: ../../images/door_sensor/aeon_recessed_b.jpg
	.. :align: left
	
Button actions
~~~~~~~~~~~~~~~~~~~
	#. Short press z-wave button: 
		Add/Remove device to/from a z-wave network
	#. Press and hold z-wave button for 6 seconds
		1, It will be wake up and send Wake Up Notification with broadcast.
		2, It will sleep after you released the z-wave button for 10 seconds, or sleep right away when received the Wake Up No More Information and then the led will turn off.
	#. Press and hold the Z-wave Button for 20 seconds
		Recessed Door Sensor will be reset and send Device Reset Locally CC to controller.
		Note: This procedure should only be used when the primary controller is inoperable or missing.

Specification
~~~~~~~~~~~~~~~~~~~~~~
	- Model number: 				ZW089 
	- Power source: 				Battery
	- Protocol: 					Z-Wave Plus
	- Battery type: 				CR2 
	- Dimension:					2 x 3 x 4 inches
	- Weight:						0.25 lb
	- Color: 						White
	
	
.. Wake up information
.. ~~~~~~~~~~~~~~~~~~~~~
	Recessed Door Sensor will keep wake up for 10 seconds after it send wake up notification command. If it’s included into Z-wave network, the Recessed Door Sensor will wake for 10 minutes.
	
	Only 2 ways can abort this status:
		#. Z-wave Button held 6 seconds, then released, after 8 seconds, sleep right now;
		#. Recessed Door Sensor received “Wake up no more information CC”, sleep immediately;

.. Link in Amazon
.. ~~~~~~~~~~~~~~~~~
	https://www.amazon.com/Recessed-Invisible-security-Battery-powered/dp/B0151Z49BO

.. Configuration description
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~
	
	#. Parameter 1: Which value of the Sensor Binary Report will be sent when the magnet switch to open/close.
		- Parameter: 1 (0x01)
		- Size: 1 byte
		- Value:
			(1) Value=0, Open=Sensor Binary Report 0xFF, Close=Sensor Binary Report 0x00.
			(2) Value=1, Open= Sensor Binary Report 0x00, Close=Sensor Binary Report 0xFF.
		- Default: 0
	
	#. Parameter 3: Which value of the Basic Set will be sent when the magnet switch to open/close.
		- Parameter: 3 (0x03)
		- Size: 1 byte
		- Value:
			(1) Value=0, Open= Basic Set 0xFF, Close=Basic Set 0x00.
			(2) Value=1, Basic Set 0x00, Close= Basic Set 0xFF.
		- Default: 0
	
	#. Parameter 101: Enable/disable the function of low battery checking, when the current voltage is less than the warning voltage, it will send the Battery Low Warning Report
		- Parameter: 101 (0x65)
		- Size: 1 byte
		- Value:
			(1) 00 = Disable
			(2) 01 = Enable
		- Default: 0
	
	#. Parameter 111: Low battery checking interval
		- Parameter 111 (0x6F)
		- Size: 4 bytes
		- Value: 0 ~ 0x7fffffff in seconds. Unit is 4 minutes.
		- Default: 0x00015270 (24 hours)
		Note: 
			(1) This parameter only will be activated after the function of low battery checking (parameter 101) is enabled.
			(2) Recessed Door Sensor also will check the current battery voltage when it was wake up as other ways such as zwave button trigger, magnet switch trigger...

	
	#. Parameter 121: Trigger report types
		- Parameter: 121 (0x79)
		- Size: 4 bytes
		- Value: bit setting
			(1) Bit 8: Basic set
			(2) Bit 4: Binary report
		- Default: 0x00000100

	#. Parameter 252: Lock configuration setting
		- Parameter: 252 (0xFC)
		- Size: 1 byte
		- Value:
			(1)  0 = Unlock
			(2) 1 = Lock
		- Default: 1
