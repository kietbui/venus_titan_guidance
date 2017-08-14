GE lighting control duplex
--------------------------------
GE Z-Wave Wireless Smart Lighting Control Duplex Receptacle Outlet, On/Off, In-Wall, White, Works with Amazon Alexa, 12721
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


	.. image:: ../../images/onoff_inwall_outlet/ge_lighting_control_duplex_12721.jpg
	.. :align: left

Key Features
~~~~~~~~~~~~~~~~~~
	- One Z-wave remote controlled AC outlet
	- Remote ON/OFF control via the Z-Wave controller/network
	- Manual ON/OFF control with the front panel pushbutton
	- One Always-ON pass through AC outlet

Basic Operation
~~~~~~~~~~~~~~~~~~~
	The connected light can be turned ON in two ways:
	- With a remote
	- Manually with the pushbutton on the Z-Wave receptacle

Specification
~~~~~~~~~~~~~~~~~~~~~~
	- Power 120VAC, 60Hz
	- Signal (Frequency) 908.42 MHz
	- Maximum load for both outlets; 1800W Resistive
	- Maximum Load for the Z-Wave controlled outlet: 600W
	- Incandescent, ½ HP Motor or 1800W (15A) Resistive
	- Range: Up to 100 feet line of sight between the Wireless Controller and the closest Z-Wave receiver module.
	- Operating Temperature Range: 32-104° F (0-40° C)
	- For indoor use only


Inclusion/Exclusion to/from a network
~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Press z-wave button once. Device will be included/excluded to/from zwave network.
		
Link in Amazon
~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	https://www.amazon.com/GE-Wireless-Lighting-Receptacle-12721/dp/B0013V1SRY
	
	
	
Configuration description
~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. LED indicator
		- Parameter: 3 (0x03)
		- Size: 1 byte
		- Value:
			(1) 0 = LED ON when turn OFF
			(2) 1 = LED OFF when turn OFF
		- Default: 0
	
