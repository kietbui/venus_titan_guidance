Fortrezz Z-Wave WWA02AA Water/Temperature Sensor
---------------------------------------

	.. image:: ../../images/water_flood/fortrezz_water_alarm.jpg
	.. :align: left
	
Product Description
~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. The WWA-02AA Z-Wave Water & Temperature Sensor with LED indicator will detect water loss and help prevent water damage caused by leaking pipes, corroded water heaters, water storage tanks, leaky faucets, refrigerator drip pans etc
	#. Visual alerts via LED (non-audible)

Working with PhD
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Monitor your Fortrezz Water/Temperature Sensor and other connected devices with the Zinno app available on iOS&Android
	#. Receive alerts from PhD if the Fortrezz Water/Temperature Sensor detects detects water, or if the temperature changes
	#. Associate Fortrezz Water/Temperature Sensor with other smart devices in Zinno App, and set them to turn on or off when sensor detects water	


Add Fortrezz Water/Temperature Sensor to PhD's network
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. On the Zinno app, press Left Menu Bar, then select “Devices”
	#. Select “+” button to put the PhD in inclusion mode, keep the sensor close to PhD within 3 feet (0.91 meter)
	#. Press and hold the Program button for approx. 2 seconds
	#. If detecting a new device successfully, PhD will announce “Found Device”, and Zinno app will display the dialog box, asking user to interact with device one more time
	#. Briefly press the Program button one more time, PhD will announce “The device is being added”
	#. If adding the sensor successfully, PhD will announce “Adding Fortrezz Flood Detected Sensor success” and on Zinno app will display the dialog boxes that indicate user has added device successfully		

	.. image:: ../../images/water_flood/fortrezz_water_alarm_d.jpg
	.. :align: left		
	
.. Inclusion/Exclusion to/from a network
.. ~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Press and hold program button in 2 seconds. Device is excluded from current zwave network
	#. To include device to open zwave network, double press program button within 1.5 seconds


.. LED indicator
.. ~~~~~~~~~~~~~~~~
	- 1 fast blink: Wake-up, notification sent (after quick button press and device is in z-wave network)
	- 2 fast blink: Water alarm
	- 3 fast blink: Temperature Alarm (either high or low setpoint triggered)
	- 4 fast blink: An active alarm has been cleared (when a water alarm or a temperature alarm is no longer active)
	- 5 fast blink: Low Battery (repeated every approx. 40 seconds)
	- 1 slow blink: Device in z-wave network (also, after button held while in-Network)
	- 3 slow blink: Device is removed from z-wave network (also given if adding was not completed)


.. Wake-up information
.. ~~~~~~~~~~~~~~~~~~~~~~
	- Wakeup1: Power saving design wakes up every 4 seconds to test water and freeze sensor
	- Wakeup2: Once every 4 approx. hours (default) unit wakes up to send a notification to controller to query and update the status of the unit. A controller can change this wakeup interval. Battery life is decreased when the wakeup interval time is shorter.



.. Link in Amazon
.. ~~~~~~~~~~~~~~~~~~~~~~~~~
	https://www.amazon.com/Wireless-Water-Temperature-Sensor-Buzzer/dp/B007TB3RWQ

.. Configuration description
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Low temperature threshold
		- Parameter: 1 (0x01)
		- Size: 1 byte
		- Value: 
			+ Valid value: 
				(1) 0x00 ~ 0x7F (from 0 ~ 127 oC)
				(2) 0xFF ~ 0x81 (from -127 ~ -1 oC)
			+ Unit is celsius
		- Default: 0x04
		
	#. High temperature threshold
		- Parameter: 2 (0x02)
		- Size: 1 byte
		- Value: 
			+ Valid value: 
				(1) 0x00 ~ 0x7F (from 0 ~ 127 oC)
				(2) 0xFF ~ 0x81 (from -127 ~ -1 oC)
			+ Unit is celsius
		- Default: 0x46
