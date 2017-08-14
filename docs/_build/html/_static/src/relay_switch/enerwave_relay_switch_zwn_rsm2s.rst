Enerwave dual relay switch module
--------------------------------
Enerwave ZWN-RSM2 Z-Wave Smart Dual Relay Switch Module, NEUTRAL WIRING REQUIRED
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


	.. image:: ../../images/relay_switch/enerwave_single_relay_zwn_rsm1s.jpg
	.. :align: left
	
Feature and benefits
~~~~~~~~~~~~~~~~~
	- Work with existing light switches, required neutral wire
	-  Slim size module with build in Z-Wave technology and Interoperable with other Z-Wave enabled devices
	- On/Off control via Z-Wave controller, manual wall switch
	- Acts as a Z-Wave repeater to extend the range
	- 3 way wiring compatible

Specification
~~~~~~~~~~~~~~~~~~~~~~
	- Voltage: 120-277VAC, 50/60Hz
	- Maximum Load requirement: 4A + 4A
	- Z-Wave Frequency: 908.42MHz
	- Operating Temperature: 32° F-104° F
	- Range: Up to 150 feet line of sight between the Wireless Controller and the closest Z-Wave receiver module. 

Inclusion/Exclusion to/from a network
~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Press program button once or the ON/OFF toggle on the switch 3 times. Device will be included/excluded to/from zwave network.
	
	.. image:: ../../images/relay_switch/enerwave_single_relay_zwn_rsm2s_d.jpg
	.. :align: left
	
		
Link in Amazon
~~~~~~~~~~~~~~~~~~~~~
	https://www.amazon.com/Enerwave-ZWN-RSM2-Z-Wave-NEUTRAL-REQUIRED/dp/B00JWVNH4Y
	
	
Configuration description
~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Timming of dim steps when all-on/all-off command
		- Parameter: 12 (0x0C)
		- Size: 2 byte
		- Value:
			1 ~ 255: number of steps
		- Default: 3
		
	
