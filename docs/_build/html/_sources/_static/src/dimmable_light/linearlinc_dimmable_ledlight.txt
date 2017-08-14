LinearLinc Dimmable LED light
--------------------------------
GoControl Z-Wave Dimmable LED Light Bulb, LB60Z-1
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

	.. image:: ../../images/dimmable_light/linearlinc_dimmable_ledlight.jpg
	.. :align: left

Basic operation
~~~~~~~~~~~~~~~~~~~~~~~~~~
	- Remote Control Operation
		The Smart LED Light Bulb can be controlled ON / OFF/ BRIGHT / DIM through wireless signals from the Z-Wave remote controller or through a gateway via an application on a smart phone, tablet, or PC.
		Once the Smart LED Light Bulb has been added to the network,depending on the functions supported by your controller, it can be assigned to a Group or Scene and operate when the ALL ON or ALL OFF command is received from the Controller. It can also be set in Association with another Z-Wave device to perform a specifi c duty.
	- Manual Operation
		The Smart LED Light Bulb can be manually operated using the wall switch while keeping it on-line with the Z-Wave network.
	- To manually turn the Smart LED Light Bulb ON:
		Flip the wall switch OFF then ON. Be sure the switch is ON when fi nished.
	- To manually turn the Smart LED Light Bulb OFF:
		Flip the wall switch OFF then ON twice within two seconds. Be sure the switch is ON when fi nished.

Specification
~~~~~~~~~~~~~~~~~~~~~~~~~~~
	- Power Supply: 120 VAC, 60 Hz
	- Brightness: 750 lumens (Equivalent to 60 Watt incandescent light bulb)
	- Power Consumption: 9 Watts
	- Color Temperature: 2700K
	- Bulb Lifetime: 25,000 hour (equivalent 22.8 years based on 3 hours/day)
	- Radio Frequency: 908.4 MHz / 916 MHz
	- Range: Up to 130 feet line of sight between the Z-Wave Controller and/or the closest Z-Wave Repeater
	- Normal Operating Temp: 77°F (25°C)
	- Repeater: Yes


Inclusion/Exclusion to/from a network
~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Power OFF then power ON device
	#. Device flashes to indicate process completes
	
Link in Amazon
~~~~~~~~~~~~~~~~~
	https://www.amazon.com/GoControl-Z-Wave-Dimmable-Light-LB60Z-1/dp/B00PJH16UC

Configuration description
~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Dim level memory
		- Parameter: 1 (0x01)
		- Size: 1 byte
		- Value: 
			0 = the bulb will be full brightness when turned on.
			1 = the bulb will turn on to the last dim level setting.
		- Default: 0
