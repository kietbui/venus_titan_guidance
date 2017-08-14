Vision In-Wall Micro Dual Relay Switch
---------------------------------

Vision In Wall Z-Wave Micro Switch, 2 relay
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

	.. image:: ../../images/relay_switch/vision_inwall_micro_2relay_zl7432.jpg
	.. :align: left
	
Operation
~~~~~~~~~~~~~~~~~
	- Turn on or turn off the appliances that attached to Controller, or manually turn on/off the light switch.

Specification
~~~~~~~~~~~~~~~~~~~~~~
	- Protocol: Z-Wave™ (ZM3102N)
	- Frequency Range:
		865.22MHz (ZL7432IN)
		868.42MHz (ZL7432EU)
		869.00MHz (ZL7432RU)
		908.42MHz (ZL7432US)
		916.00MHz (ZL7432IS)
		920.00MHz (ZL7432JP)
		921.42MHz (ZL7432BR)
	- Operating Range: Up to 100 feet line of sight
	- Operating Temp.: -15°C~ 60°C (5°F~140°F)
	- Operating Voltage: 100VAC~240VAC
	- Resistive Load:
		800W for 110VAC
		1300W for 220VAC

Inclusion/Exclusion to/from a network
~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Turn on and turn off switch that connects with ZL7432 module 4 times. Device will be included/excluded to/from zwave network.
	
	.. image:: ../../images/relay_switch/vision_inwall_micro_2relay_zl7432_d.png
	.. :align: left
	
		
Link in Amazon
~~~~~~~~~~~~~~~~~~~~~
	https://www.amazon.com/Vision-Z-Wave-Micro-Switch-relay/dp/B00R883YKU
	
	

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
