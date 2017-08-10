Vision In-Wall Micro Single Relay Switch
---------------------------------

Vision In Wall Z-Wave Micro Switch, 1 relay
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

	.. image:: ../../images/switch/vision_inwall_micro_1relay_ZL7431US.jpg
	.. :align: left
	
Operation
~~~~~~~~~~~~~~~~~
	- Turn on or turn off the appliances that attached to Controller, or manually turn on/off the light switch.

Specification
~~~~~~~~~~~~~~~~~~~~~~
	- Protocol: Z-Wave™ (ZM5101)
	- Frequency Range:
		865.22MHz (ZL7434IN-5)
		868.10MHz (ZL7434MY-5)
		868.42MHz (ZL7434EU-5)
		869.00MHz (ZL7434RU-5)
		908.42MHz (ZL7434US-5)
		916.00MHz (ZL7434IL-5)
		919~923MHz (ZL7434KR-5)
		919.80MHz (ZL7434HK-5)
		922~926MHz (ZL7434JP-5)
		921.42MHz (ZL7434BR-5)
	- Operating Range: Up to 100 feet line of sight
	- Operating Temp.: -15°C~ 60°C (5°F~140°F)
	- Operating Voltage: 100VAC~240VAC
	- Max Load:
		NO: 10A/1200W @ 120VAC
			7A/1540W @ 220VAC
		NC: 5A/600W @ 120VAC
			5A/1100W @ 220VAC 

Inclusion/Exclusion to/from a network
~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Press 3 times program switch within 2 seconds or turn on the wall switch 3 times within 2 seconds and wait for exclusion completes
	#. Press 3 times program switch within 2 seconds or turn on the wall switch 3 times within 2 seconds and wait for inclusion completes
	

Configuration description
~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Light control 
		- Parameter: 1 (0x01)
		- Size: 1 byte
		- Value:
			1 = To Control Light with 1 Wall Switch & to Control Light With 2 Wall Switches.
			2 = To Control Light with 1 Wall Switch That Has Light Indicator
		- Default: 2
	
	#. Light control 
		- Parameter: 2 (0x02)
		- Size: 1 byte
		- Value:
			1 = With common on/off type switch button used
			2 = With momentary type switch button used.
		- Default: 1
