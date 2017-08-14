Leviton Decora In-Wall Smart Dimmer
--------------------------------
Leviton DZ1KD-1BZ Decora Smart 1000W Dimmer with Z-Wave Plus Technology, White/Light Almond
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


	.. image:: ../../images/dimmable_inwall_switch/leviton_decora_inwall_dimmer_dz1kd.jpg
	.. :align: left

Operation
~~~~~~~~~~~~~~~~~
	- At default the locator light will illuminate when the load is in the OFF position to facilitate access in the dark.
	- If using the dimmer in a 3-way application, the lights will turn ON at brightness set on dimmer’s DIM/BRIGHT bar. The lighting can be controlled from either the dimmer, the remote location or a Z-Wave® enabled controller.
	- By default setting, top rocker is ON and bottom is OFF
	- Tap the TOP half of the DIM/BRIGHT Bar – Lights will jump to the next brightness setting. Hold the TOP half of the DIM/BRIGHT Bar – Lights will brighten
	- Tap the BOTTOM half of the DIM/BRIGHT Bar – Lights will jump to the next dim setting. Hold the BOTTOM half of the DIM/BRIGHT Bar – Lights will dim.
	
Specification
~~~~~~~~~~~~~~~~~~~~~~
	- Power: 120 VAC, 60 Hz.
	- Incandescent: 1000W
	- LED/CFL: 450W
	- Signal (Frequency): 908.42 MHz.


Inclusion/Exclusion to/from a network
~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Press and hold top paddle until LED changes to orange, release then press top paddle once to reset device.
	#. LED will flash orange then change to flash green indicate inclusion/exclusion process completes.
	
Link in Amazon
~~~~~~~~~~~~~~~~~~~
	https://www.amazon.com/Leviton-DZ1KD-1BZ-Decora-Dimmer-Technology/dp/B01MQX5L8P/ref=sr_1_2?s=hi&ie=UTF8&qid=1502426812&sr=1-2&keywords=Leviton+DZMX1

Configuration description
~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Fade On time
		- Parameter: 1 (0x01)
		- Size: 1 byte
		- Value:
			(1) 0 = Instant On
			(2) 1 - 127 = Seconds: 1 - 127 seconds
			(3) 128 - 253 (0x80 - 0xFD) = Minutes: 1 - 126 minutes
		- Default: 2
	
	#. Fade Off time
		- Parameter: 2 (0x02)
		- Size: 1 byte
		- Value:
			(1) 0 = Instant Off
			(2) 1 - 127 = Seconds: 1 - 127 seconds
			(3) 128 - 253 (0x80 - 0xFD) = Minutes: 1 - 126 minutes
		- Default: 2
	
	#. Minimum light level
		- Parameter: 3 (0x03)
		- Size: 1 byte
		- Value: 0 ~ 100
		- Default: 10
	
	#. Maximum light level
		- Parameter: 4 (0x04)
		- Size: 1 byte
		- Value: 0 ~ 100
		- Default: 100
		
	#. Preset light level
		- Parameter: 5 (0x05)
		- Size: 1 byte
		- Value:
			0: Last memorized dim level
			1 ~ 100: dim level
		- Default: 0
	
	#. LED Dim Level Indicator Timeout
		- Parameter: 6 (0x06)
		- Size: 1 byte
		- Value:
			0 = Level Indicators Off
			1 - 254 (0x01 - 0xFE) = Level Indicator Timeout (seconds)
			255 (0xFF) = Levels Always On
		- Default: 3
		
	#. Locator LED Status
		- Parameter: 7 (0x07)
		- Size: 1 byte
		- Value:
			0 = LED Off
			254 (0xFE) = Status Mode
			255 (0xFF) = Locator Mode
		- Default: 255
	
	#. Load type
		- Parameter: 12 (0x0C)
		- Size: 2 byte
		- Value:
			0 = Incandescent
			1 = LED
			2 = CFL
			3 = Mark 10
		- Default: 0
		
