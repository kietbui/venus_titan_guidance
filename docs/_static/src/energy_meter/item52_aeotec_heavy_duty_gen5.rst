Aeon Labs Z-Wave Plus ZW078-A Heavy Duty Smart Switch Gen5
------------------------------------------------------------------------

	.. image:: ../../images/energy_meter/aeotec_heavy_duty_gen5.jpg
	.. :align: left
	
Product Description
~~~~~~~~~~~~~~~~~~~~~~
	#. Control your heavy duty appliances, turning them on/off remotely
	#. Real-time energy monitoring and reporting
	#. Works with 40 amp appliances

Working with PhD
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Monitor and Control Aeon Labs Heavy Duty Switch Gen5 by PhD via the Zinno app available on iOS&Android
	#. Automate and schedule the operation of the high-power devices wired into the switch 
	#. Calculate and report your spend in watts and kilowatt hours in real-time
	#. In the event of an emergency, PhD can be used to turn off the electronics that Heavy Duty Smart Switch are connected to

Add Aeon Labs Heavy Duty Switch to PhD's network
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. On Zinno App, go to Menu → Devices → Tap "+" button to put PhD to inclusion mode
	#. Press Action button once. Device will be included/excluded to/from zwave network.
	
	.. image:: ../../images/energy_meter/aeotec_heavy_duty_gen5_i.jpg
	.. :align: left	
	
Specification
~~~~~~~~~~~~~~~~~~~~~
	- Model number: 				ZW078-A
	- Power rating: 				240VAC, 50/60Hz (2Phases L1,L2)
	- Current Output:				40A
	- Protocol:						Z-Wave Plus
	- Dimension:					5.9 x 4.7 x 1.6 inches
	- Weight:						1.05 pounds
	- Color: 						White


	
.. Factory reset
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~
	- Power-up device
	- Press and hold z-wave button for 20 seconds
	*Note: when hold more than 1 second, LED blinks faster and faster. When holding more than 20 seconds, LED is on in 2 seconds.*
	
.. Link in Amazon
.. ~~~~~~~~~~~~~~~
	https://www.amazon.com/Aeon-Labs-White-V3-26-AL001/dp/B00MBIRF5W

.. Configuration description
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Enable overload protection: When enable this function, load will be closed when the current more than 39.5A and the time more than 5 seconds. 
		- Parameter: 3 (0x03)
		- Size: 1 byte
		- Value: 
			+ 0x00: disable this feature
			+ 0x01: enable this feature
		- Default: 0
		
	#. LED status after power-on
		- Parameter: 20 (0x14)
		- Size: 1 byte
		- Value: 
			+ 0x00: last status
			+ 0x01: always ON
			+ 0x02: always OFF
		- Default: 0
		
	#. Enable to send notification to associated group (group 1) when load changes
		- Parameter: 80 (0x50)
		- Size: 1 byte
		- Value: 
			+ 0x00: disable this feature
			+ 0x01: hail CC
			+ 0x02: basic CC report
		- Default: 0
	
	#. Enable min change report
		- Parameter: 90 (0x5A)
		- Size: 1 byte
		- Value: 
			+ 0x00: disable this feature
			+ 0x01: enable this feature
		- Default: 1
		
	#. Enable report for threshold change (in Watt)	
		- Parameter: 91 (0x5B)
		- Size: 2 bytes
		- Value: 0 ~ 60000
		- Default: 50
		
	#. Enable report for threshold change (in percentage)
		- Parameter: 92 (0x5C)
		- Size: 1 byte
		- Value: 0 ~ 100
		- Default: 10
	
	#. Report items to Group 1
		- Parameter: 101 (0x65)
		- Size: 4 bytes
		- Value: bit setting
			+ bit 0: meter report for voltage
			+ bit 1: meter report for current
			+ bit 2: meter report for watt
			+ bit 3: meter report for kilo-watt
		- Default: 0x00000004

	#. Enable lock configuration
		- Parameter: 252 (0x5C)
		- Size: 1 byte
		- Value: 0 ~ 100
		- Default: 10


