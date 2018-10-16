Sensative Z-Wave Plus TRTCC1825 Door/Window Sensor
----------------------------------------------

	.. image:: ../../images/door_sensor/sensative_strips_door_sensor.jpg
	.. :align: left

Product Description
~~~~~~~~~~~~~~~~~~~
	#. Monitor doors, windows, gates, and cabinets from your smart home app when you're away
	#. Unlike most other door / window sensors which are mounted on the frame, Strips is so slim it fits BETWEEN the frames of any standard window or door
	#. Strips is completely sealed so it can be mounted on any non-metal surface outside

Working with PhD
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Be monitored by PhD via the Zinno app available on iOS&Android
	#. The Speaker on Phd will annouce when receive the alert from the Sensative Door/Window Sensor
	#. Associate Sensative Door/Window Sensor with other smart devices in Zinno App, and set them turn on or off if the sensor detects doors or windows have been open	

Add Sensative Door/Window Sensor to PhD's network
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. On Zinno App, go to Menu → Devices → Tap "+" button to put PhD to inclusion mode
	#. Follow process to wake device up, device will be included/excluded to/from zwave network.
		- Place the round magnet at the rounded edge.  
		- When the LED blinks, move the magnet away.  
		- Repeat 3 times in total within 10 seconds. 
	
	.. image:: ../../images/door_sensor/sensative_strips_door_sensor_wk1.jpg
	.. :align: left
	.. image:: ../../images/door_sensor/sensative_strips_door_sensor_wk2.jpg
	.. :align: left

Specification
~~~~~~~~~~~~~~~~~~~~~~
	- Model number: 				TRTCC1825  
	- Power source: 				Battery
	- Protocol: 					Z-Wave Plus
	- Battery type: 				(Custom Made Battery) 
	- Dimension:					7.68 x 0.59 x 0.12 inches
	- Weight:						0.07 lb
	- Color: 						White & Brown	

	
.. LED indication
.. ~~~~~~~~~~~~~~~~~~
	- 1 short blink		User feedback during commands 
						Specific event detected (E.g door opened)
	- 2 short   		For demo purposes (only if Strips is not added) 
	- 1 long   			User command successfully executed 
	- 5 short   		Error. E.g. communication with controller failed
	
.. Factory reset
.. ~~~~~~~~~~~~~~~
	 You may reset Strips if the controller is lost. Follow the instructions above for Wake up. After 5 LED blinks, place the magnet at the rounded edge again for 10 seconds. A long LED signal indicates success. 
	
.. Link in Amazon
.. ~~~~~~~~~~~~~~~~
	 https://www.amazon.com/Sensative-Strips-Z-Wave-Window-Contact/dp/B01LWMTUI8


.. Configuration description
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Notification type
		- Parameter: 1 (0x01)
		- Size: 1 byte
		- Value:
			(1) 0 = Binary sensor report
			(2) 1 = Notification report
			(3) 2 = Basic set report
		- Default: 1
		
	#. LED indication
		- Parameter: 2 (0x02)
		- Size: 1 byte
		- Value:
			(1) 0 = Disable LED for specific event
			(2) 1 = Enable LED for specific event
