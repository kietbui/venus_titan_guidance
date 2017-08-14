Enerwave in-wall switch
--------------------------------
Enerwave Z-Wave ZW15S Wireless Lighting 3-Way Switch, Works with Alexa Voice Control, NEUTRAL REQUIRED
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


	.. image:: ../../images/onoff_inwall_switch/enerwave_inwall_switch_zw15s.jpg
	.. :align: left

Specification
~~~~~~~~~~~~~~~~~~~~~~
	- Power: 120V, 60Hz
	- Incandescent: 1000W
	- Ballast: 1200VA
	- Resistive: 1800W (15A)
	- Motor: 1/2 HP
	- Z-wave frequency: 908.42 MHz
	- Operating temp: 32 ~ 104 oF
	- Range: up to 100 feet line of sign

Inclusion/Exclusion to/from a network
~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Push bottom or bottom paddle once. Device will be included/excluded to/from zwave network.
	
	.. image:: ../../images/onoff_inwall_switch/enerwave_inwall_switch_zw15s_d.jpg
	.. :align: left

	
Reference link
~~~~~~~~~~~~~~~~~~~~~~
	http://enerwaveautomation.com/products/zw15s/
	
	
Configuration description
~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. LED light specify
		- Parameter: 1 (0x01)
		- Size: 1 byte
		- Value:
			(1) 0 = LED on when light off
			(2) 1 = LED on when light on
		- Default: 0
	
	#. Invert switch
		- Parameter: 2 (0x02)
		- Size: 1 byte
		- Value:
			(1) 0 = ON at the top and OFF at the bottom
			(2) 1 = ON at the bottom and OFF at the top
		- Default: 0
