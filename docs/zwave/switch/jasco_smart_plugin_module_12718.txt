Jasco smart plugin module
--------------------------------
GE Z-Wave Wireless Smart Lighting Control Lamp Module, Dimmer, Plug-In, White, Works with Amazon Alexa, 12718
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

	.. image:: ../../images/switch/jasco_smart_plugin_module_12718.jpg
	.. :align: left

Brief information
~~~~~~~~~~~~~~~~~~
	- One Z-wave controlled AC outlet for standard incandescent lighting or dimmable CFL/LEDs
	- Remote ON/OFF and brightness control via the Z-Wave controller
	- Manual ON/OFF and brightness control with the front panel push button
	- Load-sensing turns the light ON if the switch on the connected light is used instead of the remote or push button on the Z-Wave smart switch (default setting is disabled)
	- One always-on pass-through AC outlet
	- Space efficient design
	- Does not block the lower outlet when plugged in to the upper outlet of a duplex wall receptacle. (This assumes that the duplex receptacle is mounted with the ground pin down).
	- Plugs and cords for connected devices route to the side allowing close placement of furniture
	- Grounded 3-wire power connection for safety

Specification
~~~~~~~~~~~~~~~~~~~~~~
	- Power 120VAC, 60Hz
	- Maximum Load for both outlet 15A, 1800W resistive
	- Maximum load for the Z-Wave controlled outlet: 2.5A; 300W Incandescent or 100W Dimmable CFL/LED
	- Up to 100 feet line of sight between the Wireless Controller and the closest Z-Wave receiver module.
	- Operating Temperature Range: 32–104° F (0–40° C)
	- Indoor use only


Inclusion/Exclusion to/from a network
~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Press program button once to reset device
	#. Wait for confirmation from Venus/Titan and then push once again
	#. Wait for controller completes inclusion/exclusion process
	
Configuration description
~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Number of dim steps when receiving zwave command
		- Parameter: 7 (0x07)
		- Size: 1 byte
		- Value:
			1 ~ 99: number of steps
		- Default: 1
	
	#. Timming of dim steps when receiving zwave command
		- Parameter: 8 (0x08)
		- Size: 2 byte
		- Value:
			1 ~ 255: number of steps
		- Default: 3
		
	#. Number of dim steps when manual control
		- Parameter: 9 (0x09)
		- Size: 1 byte
		- Value:
			1 ~ 99: number of steps
		- Default: 1
	
	#. Timming of dim steps when manual control
		- Parameter: 10 (0x0A)
		- Size: 2 byte
		- Value:
			1 ~ 255: number of steps
		- Default: 3
		
	#. Number of dim steps when all-on/all-off command
		- Parameter: 11 (0x0B)
		- Size: 1 byte
		- Value:
			1 ~ 99: number of steps
		- Default: 1
	
	#. Timming of dim steps when all-on/all-off command
		- Parameter: 12 (0x0C)
		- Size: 2 byte
		- Value:
			1 ~ 255: number of steps
		- Default: 3
		
	#. Load sensing
		- Parameter: 29 (0x1D)
		- Size: 1 byte
		- Value:
			0 = Disable feature
			1 = Enable feature
		- Default: 3
		
