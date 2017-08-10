GoControl single inwall outlet
--------------------------------
GoControl WO15Z-1 Z-Wave Single Wall Outlet, White
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


	.. image:: ../../images/switch/gocontrol_single_inwall_outlet_wo15z1.jpg
	.. :align: left

Basic control
~~~~~~~~~~~~~~~~~~
	- Button (Local Control): The button on the WO15Z-1 allows the user to turn the load attached to the controlled outlet ON or OFF.
		• Tapping button toggles the load attached ON or OFF.
		• Include or exclude the module from the Z-Wave system.
		When a Controller prompts to “Send Node ID” or to “Press Button on Unit”, quickly tap the button once to satisfy those instructions. (Tapping the button also toggles the load attached ON or OFF).
	- Remote Control: The WO15Z-1 will respond to BASIC and BINARY commands that are part of the Z-Wave system. Refer to your Controller’s instructions as to whether your Controller can transmit those commands.

Specification
~~~~~~~~~~~~~~~~~~~~~~
	- Power 120VAC, 60Hz
	- Signal (Frequency) 908.42 MHz
	- Max load: Resistive: 15 amps (1800 watts) maximum, 120 VAC
	- Range: Up to 100 feet line of sight between the Controller and or closest Z-Wave Receiver module.


Inclusion/Exclusion to/from a network
~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Press program button once to reset device
	#. Wait for confirmation from Venus/Titan and then push once again
	#. Wait for controller completes inclusion/exclusion process
	
Configuration description
~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. LED indicator
		- Parameter: 3 (0x03)
		- Size: 1 byte
		- Value:
			(1) 0 = LED ON when turn ON
			(2) 1 = LED OFF when turn ON
		- Default: 0
	
