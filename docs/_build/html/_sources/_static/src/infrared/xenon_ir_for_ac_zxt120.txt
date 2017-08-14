Xenon IR extender for air conditioners
--------------------------------
Remotec Z-Wave ZXT-120 IR Extender for Air Conditioners
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


	.. image:: ../../images/infrared/xenon_ir_for_ac_zxt120.jpg
	.. :align: left
	
Operation
~~~~~~~~~~~~~~~~~
	- Plug-in 5Vdc power into the USB socket if operated at Always Listening mode
	- Install 3xAAA batteries if operated at FLiRS mode
	- To switch from FLiRS mode to Always listening mode, below steps are required:
		(1) Press and hold the PROG button on the ZXT-120 for around 5 seconds. LED turns ON after PROG key hold for 5seconds
		(2) Release the button and then press the PROG button 3 times within 2 seconds. LED flashes four times then stay off
	- To switch from Always listening mode to FLiRS mode, below steps are required:
		(1) Press and hold the PROG button on the ZXT-120 for around 5 seconds. LED turns ON after PROG key hold for 5seconds
		(2) Release the button and then press the PROG button 3 times within 2 seconds. LED flashes twice then stay off 

Specification
~~~~~~~~~~~~~~~~~~~~~~
	- RF operating range: up to 80 feet line of sign
	- IR operating range: up to 25 feet line of sign
	- Measure temperature range: 32 ~ 104 oF (0 ~ 40 oC)
	- Operating temperature range: 32 ~ 104 oF (0 ~ 40 oC)
	- Usb power: 5V DC - 100mA
	- Battery: 3x1.5V AAA

Inclusion/Exclusion to/from a network
~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Press program button once. Device will be included/excluded to zwave network.
	
	
Link in Amazon
~~~~~~~~~~~~~~~
	https://www.amazon.com/Remotec-Z-Wave-ZXT-120-Extender-Conditioners/dp/B00Q6SXTPS
	
Configuration description
~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Location for IR code learning and start learning
		- Parameter: 25 (0x19)
		- Size: 1 byte
		- Value: 0x00 ~ 0x16
		- Default: N/A
	
	#. Learning status
		- Parameter: 26 (0x1A)
		- Size: 1 byte
		- Value: 
			+ 0x00: idle, target channel is idle
			+ 0x01: OK, the latest learning process successful and completed
			+ 0x02: learning, ZXT-120 is busy
			+ 0x04: failed, the latest learning request failed
		- Default: 0x00
	
	#. IR code number for built-in code lib
		- Parameter: 27 (0x1B)
		- Size: 1 byte
		- Value: 
			Refer to "Code list" for setting value
		- Default: N/A
	
	#. External IR emitter power level
		- Parameter: 28 (0x1C)
		- Size: 1 byte
		- Value: 
			+ 0x00: normal power mode
			+ 0xFF: high power mode
		- Default: 0xFF
	
	#. Surround IR control
		- Parameter: 32 (0x20)
		- Size: 1 byte
		- Value: 
			+ 0x00: disable surround IR emitters
			+ 0xFF: enable surround IR emitters
		- Default: 0xFF
	
	#. AC function swing control
		- Parameter: 33 (0x21)
		- Size: 1 byte
		- Value: 
			+ 0x00: swing OFF
			+ 0xFF: swing auto
		- Default: 0xFF
	
	#. Sensor temperature compensation
		- Parameter: 37 (0x25)
		- Size: 1 byte
		- Value: 
			+ 0x00 ~ 0x7F: compensation temperature from 0 ~ 127 oC
			+ 0x80 ~ 0xFF: compensation temperature from -127 ~ -1 oC
		- Default: 0x00
	
	
