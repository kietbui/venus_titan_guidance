Aeotec LED bulb gen5
--------------------------------
Aeotec by Aeon Labs ZW098 Aeon Labs LED Bulb, Small, White
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

	.. image:: ../../images/dimmable_light/aeotec_led_zw098.jpg
	.. :align: left

Brief information
~~~~~~~~~~~~~~~~~~~~~~~~~~
	- Aeon labs LED bulb is a swith multilevel device based in z-wave.
	- The bulb has 5 main colors: red, green, blue, warm white and cold white
	- Has repeater role in z-wave mess network
	- Can be upgrade firmware via OTA

Specification
~~~~~~~~~~~~~~~~~~~~~~~~~~~
	- Bulb holder type: E26 for US version, E27 for EU/AU version
	- Max operation power: 9W
	- Max standby power: 0.7W
	- Operating temperature: -10 ~ 45 oC
	- Relative humidity: 8 ~ 80%
	- Operating range: up to 500 feet/150 meters


Inclusion/Exclusion to/from a network
~~~~~~~~~~~~~~~~~~~~~~~
	#. LED bulb must be installed with external switch
	#. Put controller to Inclusion/Exclusion mode
	#. Turn off then turn on (via external switch), repeat 3 times within 2 seconds
	#. LED will change its color to indicate include/exclude completes
	
	.. image:: ../../images/dimmable_light/aeotec_led_zw098_e.jpg
	.. :align: left

Link in Amazon
~~~~~~~~~~~~~~~~~~~
	https://www.amazon.com/Aeotec-Aeon-Labs-ZW098-Small/dp/B00VQISQW4

Configuration description
~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Enable function of using external switch to turn on/off 
		- Parameter: 34 (0x22)
		- Size: 1 byte
		- Value: 
			0x00: enable
			0x01: disable
		- Default: 0x00
	
	#. Enable function of using external switch to change color
		- Parameter: 35 (0x23)
		- Size: 1 byte
		- Value: 
			0x00: enable
			0x01: disable
		- Default: 0x01
	
	#. Enable to send notification to associated devices (group 1) when LED state is changed
		- Parameter: 80 (0x50)
		- Size: 1 byte
		- Value: 
			0x00: nothing
			0x01: hail CC
			0x02: basic CC report
		- Default: 0x01 - for US version and 0x02 for others
	
	#. Lock configuration
		- Parameter: 252 (0xFC)
		- Size: 1 byte
		- Value: 
			0x00: un-lock configuration
			0x01: lock configuration
		- Default: 0
	
	
