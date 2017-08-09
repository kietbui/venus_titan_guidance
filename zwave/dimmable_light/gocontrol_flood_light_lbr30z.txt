GoControl dimmable flood light
--------------------------------
GoControl Bulbz Z-Wave Dimmable BR30 LED Indoor Flood Light - LBR30Z-1
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

	.. image:: ../../images/dimmable_light/gocontrol_flood_light_lbr30z.jpg
	.. :align: left

Features & benefits
~~~~~~~~~~~~~~~~~~~~~~~~~~
	- Uses only 7.5 watts of energy and provides as much light as a traditional 65-watt incandescent flood light bulb (650 lumens)
	- Medium-cool 5,000K light appearance (pleasant and cool, providing near-daylight illumination)
	- Perfect for recessed ‘can’ (4" or larger) and track light fixtures that use flood lights; for kitchens, bathrooms, family & living rooms, foyers, offices - you name it
	- Annual energy consumption (@ 3 hrs./day, 11¢/kWh) is only $0.90!
	- Includes wall light switch ‘clip’ that will keep the light switch in the ‘on’ position to ensure that the Z-Wave circuitry inside the flood light bulb is always active
	- Dimensions: 3.75" diameter by 5.375" high

Specification
~~~~~~~~~~~~~~~~~~~~~~~~~~~
	- Power Supply: 120 VAC, 60 Hz
	- Brightness: 650 lumens (Equivalent to 65 Watt incandescent light bulb)
	- Power Consumption: 7.5 Watts
	- Color Temperature: 5000K
	- Bulb Lifetime: 25,000 hour (equivalent 22.8 years based on 3 hours/day)
	- Radio Frequency: 908.4 MHz / 916 MHz
	- Wireless Range: Up to 130 feet line of sight between the Z-Wave Controller and/or the closest Z-Wave Repeater
	- Normal Operating Temp 77°F (25°C)
	- Repeater Yes


Inclusion/Exclusion to/from a network
~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Power on device and wait for exclusion completes
	#. Power on device and wait for inclusion completes

Configuration description
~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Dim level memory
		- Parameter: 1 (0x01)
		- Size: 1 byte
		- Value: 
			+ 0x00: the bulb will be full brightness when turned on.
			+ 0x01: the bulb will turn on to the last dim level setting.
		- Default: 0x00
	
	#. Dim/Bright step level
		- Parameter: 9 (0x09)
		- Size: 1 byte
		- Value: 0x01 ~ 0x63
		- Default: 0x01
	
	#. Dim/Bright speed
		- Parameter: 10 (0x0A)
		- Size: 1 byte
		- Value: 0x01 ~ 0x0A
		- Default: 0x03
	
	
