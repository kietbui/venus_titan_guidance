Honeywell YTH8320ZW1007/U Z-Wave Enabled Programmable Thermostat
----------------------------------------------------------------------

	.. image:: ../../images/themostat/honeywell_programmable.jpg
	.. :align: left

Brief information
~~~~~~~~~~~~~~~~~~~~~~~~~
	- One-touch temp control overrides program schedule at any time.
	- Precise comfort control keeps temperature within 1°F of the level you set.
	- Change/check reminders let you know when to service or replace filters and other critical components.
	- Large touchscreen display with backlight is easy to read—even in the dark.
	- Z-Wave wireless control lets you connect the thermostat to a Z-Wave network.

How to add to VENUS app  
~~~~~~~~~~~~~~~~~~~~~~~

	**1. Activation**
		- Press "Add button" (button '+') in app
		- Remove the plastic pull-tab from the back of device
		- Press SYSTEM button
		- Press and hold blank center key until the display changes
		- Change the setting:
			+ Function: RF10
			+ Setting: 1
		- Press DONE to exit and save changes
		- Wait for VENUS scan & detect this device and inform in app
	
	**2. Reset then re-add**
		- Press "Add button" (button '+') in app
		- Press SYSTEM button
		- Press and hold blank center key until the display changes
		- Change the setting:
			+ Function: RF10
			+ Setting: 0 (remove device from z-wave network)
		- Press DONE to exit and save changes
		- Press SYSTEM button
		- Press and hold blank center key until the display changes
		- Change the setting:
			+ Function: RF10
			+ Setting: 1 (add device from z-wave network)
		- Press DONE to exit and save changes
		- Wait for VENUS scan & detect this device and inform in app
	
	.. image:: ../../images/themostat/honeywell_programmable_adv_setting.png
	.. :align: center
	
Reference to control
~~~~~~~~~~~~~~~~~~~~~~~~
	.. image:: ../../images/themostat/honeywell_programmable_d1.png
	.. :align: center

Reference to status display
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	.. image:: ../../images/themostat/honeywell_programmable_d2.png
	.. :align: center


Basic setting
~~~~~~~~~~~~~~~~
	#. Clock setting
	
		- Press CLOCK button
		- Press up/down button to adjust time (press and hold to advance the time more quickly)
		- Press DONE to save and exit
		
	#. Fan setting
		
		- Press FAN to select fan operation
		- Select:
			+ ON: fan is always on
			+ Auto: fan run only when the heating or cooling systems is on
			+ Circ: fan runs randomly about 35% of the time
		- Press DONE to save and exit
	
	#. System setting
	
		- Press SYSTEM button
		- Select:
			+ Heat: thermostat controls only the heating system
			+ Cool: thermostat controls only the cooling system
			+ Off: heating and cooling systems are off
			+ Auto: thermostat automatically selects heating or cooling depending on the indoor temperature
			+ Em heat: thermostat controls emergency and auxiliary heat
		- Press DONE to save and exit
	
	
Advance setting
~~~~~~~~~~~~~~~~~~~
	#. Common setting steps
		
		- Press SYSTEM button
		- Press and hold center blank button until display change
		- Change Function and Setting 
		- Press DONE to save and exit
	
	#. Function and setting list
	
		================================	========================	======================================================
		Year setting				Function: 0120			20, 21 - Year 20xx, 21xx
		Year setting				Function: 0130			01 ~ 99 - ie: 2001, 2199
		Month setting				Function: 0140			1 ~ 12 - From Jan to Dec
		Date setting				Function: 0150			1 ~ 31 - Date in month
		Schedule on/off				Function: 0160			0/4 - None programmable/Programmable
		Restore energy saving schedule		Function: 0165			0/1 - No restore/Restore
		Continuous backlight			Function: 0280			0/1 - Not set/Set continuous backlight
		Temperature format			Function: 0320			0/1 - Farenheit/Celcius
		Enable daylight saving time		Function: 0330			0/1 - Disable/Enable
		Furnace filter change reminder		Function: 0500			0 - off
		
											1 - 10 days run time (about 1 month)
											
											2 - 30 days run time (about 3 month)
											
											3 - 60 days run time (about 6 month)
											
											4 - 90 days run time (about 9 month)
											
											5 - 120 days run time (about 1 year)
											
											6 - 180 days run time (about 1.5 years)
											
											7 - 270 days run time (about 2 years)
											
											8 - 365 days run time (about 3 years)
											
											9 - 30 calendar days
											
											10 - 60 calendar days
											
											11 - 90 calendar days
											
											12 - 120 calendar days
											
											13 - 180 calendar days
											
											14 - 365 calendar days
		UV lamp replacement reminder		Function: 0520			0 - off
		
											1 - 365 days
											
											2 - 720 days
		Adaptive interlligent recovery		Function: 0530			0/1 - On/Off function
		Program schedule periods		Function: 0540			2 - 2 program periods (Wake, Sleep)
		
											4 - 4 program periods (Wake, Leave, Return, Sleep)
		Heat energy saving setpoint		Function: 0615			65 - 40~90 oF
		
											18.5 - 4.5~32 oC
		Cool energy saving setpoint		Function: 0615			78 - 50~99 oF
		
											25.5 - 10~37 oC
		Clock format				Function: 0640			12 - 12 hours format
		
											24 - 24 hours format
		Screen lock				Function: 0670			0 - Screen is unlocked
		
											1 - All functions locked except temperature controls and CANCEL key
											
											2 - Screen is fully locked
		Z-Wave inclusion/exclusion		Function: RF10			0/1 - Exclude/Include
		Share Z-Wave node information		Function: RF20			0/1 - Idle/Send node
		================================	========================	======================================================
