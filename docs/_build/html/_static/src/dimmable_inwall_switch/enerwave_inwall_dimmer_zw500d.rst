Enerwave in-wall dimmer
--------------------------------
Enerwave ZW500D-W Z-Wave Wireless 3 Way Smart LED Light Dimmer Switch, NEUTRAL REQUIRED
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


	.. image:: ../../images/dimmable_inwall_switch/enerwave_inwall_dimmer_zw500d.jpg
	.. :align: left

Operation
~~~~~~~~~~~~~~~~~
	Enerwave ZW500D Z-wave 500W Preset Dimmer Switch is a perfect wireless manual and remote on/off/dim/bright control replacement of regular on/off and dimmer switch, controlling incandescent, dimmable LED and CFL. This Z-Wave dimmer switch is fully compatible with other Z-wave devices, provides programmable function creating a perfect ambiance such as scenes, association, schedule event, etc

Specification
~~~~~~~~~~~~~~~~~~~~~~
	- Voltage: 120VAC, 60Hz
	- Maximum load 500W Incandescent, Dimmable LED and CFL, suggested 10W or two light bulbs minimum
	- Signal Frequency: 908.42 Mhz
	- Range: Up to 100 feet in open-air and line of sight distance, depending on obstacles and blocks
	- Terminations 5 Terminals for Line, Neutral, Load, Traveler and Ground
	- Operation Temperature 32°F – 104°F (0°C -40 °C), Indoor Use

Inclusion/Exclusion to/from a network
~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Push top or bottom paddle once to reset device. Device will be included/excluded to/from zwave network.
	
Link in Amazon
~~~~~~~~~~~~~~~~
	https://www.amazon.com/Enerwave-Automation-ZW500DM-PLUS-Wireless-Interchangeable/dp/B06X9DS5TK

Configuration description
~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. LED light indication
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
