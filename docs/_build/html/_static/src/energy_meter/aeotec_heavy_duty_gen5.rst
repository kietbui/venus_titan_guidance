Heavy Duty Smart Switch Gen5
------------------------------------------------------------------------
Aeon Labs ZW078-A,White,V3.26,US,AL001 Zw078-A Z-Wave Heavy Duty Smart Energy Appliance Switch, Small, White
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

	.. image:: ../../images/energy_meter/aeotec_heavy_duty_gen5.jpg
	.. :align: left
	

Brief information
~~~~~~~~~~~~~~~~~~~~~~~~~
	- Heavy Duty Smart Switch Gen5 is an on/off switch module that also provides energy metering.
	- Z-Wave Certification ID: ZC10-14090014
	- Frequency Region: U.S./Canada/Mexico, Z-Wave Library Version: 6.51.01
	- Device Categories: All Lighting Devices,On/Off Switches/Devices

Specification
~~~~~~~~~~~~~~~~~~~~~~
	- Input: 220V~240, 60Hz. (USA Version)
             220V~240, 50Hz. (EU, AU Version)
	- Output: 220V~240, 60Hz, Max 40A Resistor load. (USA Version）
			  220V~240, 50Hz, Max 40A Resistor load. (EU Version）
			  220V~240, 50Hz, Max 40A Resistor load. (AU Version）
	- Operating temp: 5℃ - 40℃
	- Relative humidity: 8 ‐ 80%
	- Operating distance: Up to 600 feet/150 meters outdoors.

Inclusion/Exclusion to/from a network
~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Press z-wave button once. Device will be included/excluded to/from zwave network.
	
		
	.. image:: ../../images/energy_meter/aeotec_heavy_duty_gen5_i.jpg
	.. :align: left
	
Factory reset
~~~~~~~~~~~~~~~~~~~~~~~~~~
	- Power-up device
	- Press and hold z-wave button for 20 seconds
	*Note: when hold more than 1 second, LED blinks faster and faster. When holding more than 20 seconds, LED is on in 2 seconds.*
	
Link in Amazon
~~~~~~~~~~~~~~~
	https://www.amazon.com/Aeon-Labs-White-V3-26-AL001/dp/B00MBIRF5W

Configuration description
~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Enable overload protection: When enable this function, load will be closed when the current more than 39.5A and the time more than 5 seconds. 
		- Parameter: 3 (0x03)
		- Size: 1 byte
		- Value: 
			+ 0x00: disable this feature
			+ 0x01: enable this feature
		- Default: 0
		
	#. LED status after power-on
		- Parameter: 20 (0x14)
		- Size: 1 byte
		- Value: 
			+ 0x00: last status
			+ 0x01: always ON
			+ 0x02: always OFF
		- Default: 0
		
	#. Enable to send notification to associated group (group 1) when load changes
		- Parameter: 80 (0x50)
		- Size: 1 byte
		- Value: 
			+ 0x00: disable this feature
			+ 0x01: hail CC
			+ 0x02: basic CC report
		- Default: 0
	
	#. Enable min change report
		- Parameter: 90 (0x5A)
		- Size: 1 byte
		- Value: 
			+ 0x00: disable this feature
			+ 0x01: enable this feature
		- Default: 1
		
	#. Enable report for threshold change (in Watt)	
		- Parameter: 91 (0x5B)
		- Size: 2 bytes
		- Value: 0 ~ 60000
		- Default: 50
		
	#. Enable report for threshold change (in percentage)
		- Parameter: 92 (0x5C)
		- Size: 1 byte
		- Value: 0 ~ 100
		- Default: 10
	
	#. Report items to Group 1
		- Parameter: 101 (0x65)
		- Size: 4 bytes
		- Value: bit setting
			+ bit 0: meter report for voltage
			+ bit 1: meter report for current
			+ bit 2: meter report for watt
			+ bit 3: meter report for kilo-watt
		- Default: 0x00000004

	#. Enable lock configuration
		- Parameter: 252 (0x5C)
		- Size: 1 byte
		- Value: 0 ~ 100
		- Default: 10


