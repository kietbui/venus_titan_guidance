Enerwave duplex receptacle outlet
--------------------------------
Enerwave ZW15R Z-Wave Wireless Duplex Outlet 15A Tamper Resistant Receptacles, 2 Free Wall Plates
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


	.. image:: ../../images/switch/enerwave_duplex_receptacle_zw15r.jpg
	.. :align: left

Features
~~~~~~~~~~~~~~~~~~
	- Perfect replacement for regular receptacles, 120VAC, 15 Amp
	- Wireless Z-Wave technology creates a mesh network for command and
	- control interoperability with other Z-Wave compliant controller and devices
	- Manual and Remote ON/OFF control of any connected lighting and other electrical load for Z-Wave controlled outlet
	- Tamper-Resistant (TR) Receptacles keep you and your family safe
	- Reduce energy consumption and enjoy Wireless Home Automation
	- Enhance the value and technology of your condominiums and homes
	- Measures energy usage of any connected appliance/device

Specification
~~~~~~~~~~~~~~~~~~~~~~
	- Power 120VAC, 60Hz
	- Incandescent: 1000W
	- Ballast: 1200VA
	- Resistive: 1800W (15A)
	- Motor: 1/2 HP
	- Signal (Frequency) 908.42 MHz
	- Range: Up to 100 feet line of sight between the Wireless Controller and the closest Z-Wave receiver module.
	- Operating Temperature Range: 32-104° F (0-40° C)


Inclusion/Exclusion to/from a network
~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Press program button once to reset device
	#. Wait for confirmation from Venus/Titan and then push once again
	#. Wait for controller completes inclusion/exclusion process
	
Configuration description
~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. LED indicator
		- Parameter: 1 (0x01)
		- Size: 1 byte
		- Value:
			(1) 0 = LED ON when turn OFF
			(2) 1 = LED OFF when turn OFF
		- Default: 0
	
	#. Send Meter report interval (instant energy)
		- Parameter: 8 (0x08)
		- Size: 1 byte
		- Value:
			(1) 0 = Not send
			(2) 1 ~ 255: minutes
		- Default: 0
		
	#. Send Sensor multilevel report
		- Parameter: 9 (0x09)
		- Size: 1 byte
		- Value:
			(1) 0 = Not send
			(2) 1 ~ 255: minutes
		- Default: 0
		
		
	#. Send Meter report interval (accumulated energy)
		- Parameter: 10 (0x0A)
		- Size: 1 byte
		- Value:
			(1) 0 = Not send
			(2) 1 ~ 255: minutes
		- Default: 0
		
	#. Enable automatic notification to associated device when wattage changes
		- Parameter: 11 (0x0B)
		- Size: 1 byte
		- Value:
			(1) 0 = Not report
			(2) 1 = Send meter report only
			(3) 2 = Send sensor multilevel report only
			(4) 3 = Send both report
		- Default: 1
		
	#. Minimum change in wattage report
		- Parameter: 12 (0x0C)
		- Size: 1 byte
		- Value: 0 ~ 255 (0 ~ 25.5 watt)
		- Default: 10
