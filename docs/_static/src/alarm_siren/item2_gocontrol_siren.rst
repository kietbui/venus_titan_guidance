GoControl Z-Wave WA105DBZ-1 Siren and Strobe
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

	.. image:: ../../images/alarm_siren/item2_gocontrol_siren.jpg
	.. :align: left
	
Product Description
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. GoControl Siren and Strobe is for a smart, secure and safe home
	#. 105 dB alarm
	#. White LED with red lens stroke
	#. Back-up battery for the Siren keep working even when the power is out, up to 5 days (with no alarms)

Working with PhD
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Control your GoControl Z-Wave WA105DBZ-1 Siren and other connected devices with the Zinno app available on iOS&Android
	#. Associate GoControl Z-Wave WA105DBZ-1 Siren with other smart devices in Zinno App, such as door/window sensor or motion sensor... Then set the Siren on when doors or windows are opened unexpectedly, when there’s movement in your home...
	
Specification
~~~~~~~~~~~~~~~~~~~~~~
	- Model number: 				WA105DBZ-1
	- Power source: 				Battery, 100 - 240 VAC (50/60 Hz)
	- Audible Alarm: 				105 dB
	- Protocol: 					Z-Wave
	- Battery type: 				6V NiMH, 150 mAH
	- Dimension:					5.4 x 4.7 x 3.4 inches
	- Weight:					11.2 ounces
	
.. Specification
.. ~~~~~~~~~~~~~~~~~~~~~~
..	Power Supply		4 Type “AA” Alkaline batteries
..	Frequency			908.42 MHz
..	Audible Alarm		>105 dB @ 3 feet
..	Strobe				White LED with red lens
..	Operating Temp		5°F~140°F / -15°C~ 60°C
..	Repeater			No
..	Range				Up to 100 feet line of sight between the Z-Wave Controller and/or the closest Z-Wave Repeater

.. Basic operation
.. ~~~~~~~~~~~~~~~~~~~~~~
..	When triggered, the siren/strobe will trigger for 30 seconds (default setting).
..	During that time the siren will emit a very loud pulsating audible alarm at 105 db. 
..	The integrated strobe light will also flash during the 30 seconds.
..	**CAUTION:** This is an extremely loud siren, do not place it near your ear.

..	.. image:: ../../images/alarm_siren/gocontrol_siren_detail_1.jpg
..	.. :align: left

.. Include/Exclude to/from a network
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
..	#. Put controller to "Inclusion" mode
	#. Place the siren/strobe within 3 feet of the Controller 
	#. Press Program/Tamper switch for 1 second then release. The LED will blink to indicate include/exclude process completes

.. Configuration description
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~
.. 	#. Parameter 0: Siren / Strobe Mode
.. 		By default, the siren and strobe will activate when turned on. To activate the Siren only, set parameter 0 to 1. For .. .. strobe only set to 2.
.. 		- Parameter No: 0
..		- Length: 1 Byte
..		- Valid Values = 0 (default) or 1 or 2. Default is 0.
..	#. Parameter 1: Auto Stop Time
..		By default the auto stop time is 30 seconds. Setting parameter 1 to 1 will increase the time to 60 seconds. Changing it to 2 will increase the stop time to 120 seconds. Setting the stop time to 3 will turn off the auto stop and will require a command from the Controller to turn the siren/strobe off.
..		- Parameter No: 1
..		- Length: 1 Byte
..		- Valid Values = 0 or 1 or 2 or 3. Default is 0.
