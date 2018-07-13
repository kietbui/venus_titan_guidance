Vision Z-Wave ZL743US Dual Relay Switch
---------------------------------

	.. image:: ../../images/relay_switch/vision_inwall_micro_2relay_zl7432.jpg
	.. :align: left
	
Product Description
~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Extremely small factor - fits all existing double gang box
	#. Designed to work with regular light switch
	#. Simply connect the device to your existing wall switch, following the steps in instruction manual - NEUTRAL WIRE REQUIRED

Working with PhD
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Control your Vision Dual Relay Switch and other connected devices with the Zinno app available on iOS&Android
	#. With PhD, you could automatically turn Vision Dual Relay Switch on or off in many scenarios, such as door opens/closes, motion detects, and much more
	#. Also, you can automate the Vision Dual Relay Switch with PhD Scence routes, like Good Morning, Goodnight...	
	#. Control Vision Dual Relay Switch with voice commands using PhD and the Google Assistant or Amazon Alexa	

Add Enerwave Dual Relay Switch to PhD's network
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. On the Zinno app, press Left Menu Bar, then select “Devices”
	#. Select “+” button to put the PhD in inclusion mode, keep the switch close to PhD within 10 feet (3 meters)
	#. Turn on and turn off switch that connects with ZL7432 module 4 times
	#. If detecting a new device successfully, PhD will announce “Found Device”, and Zinno app will display the dialog box, asking user to interact with device one more time
	#. Repeat step #3, PhD will announce “The device is being added”
	#. If adding the sensor successfully, PhD will announce “Adding Vision In-Wall Dual Relay Switch success” and on Zinno app will display the dialog boxes that indicate user has added device successfully	

	.. image:: ../../images/relay_switch/vision_inwall_micro_2relay_zl7432_d.png
	.. :align: left

Specification
~~~~~~~~~~~~~~~~~~~~~~
	- Model number: 				ZL743US
	- Power source: 				Wall-Powered, 90VAC~265VAC , 50/60Hz
	- Resistive Load: 				800W for 110VAC, 1300W for 220VAC
	- Protocol: 					Z-Wave
	- Dimension:					1.26 x 1.5 x 0.87 inches
	- Weight:						0.1 pounds
	- Color: 						White
	
.. Specification
.. ~~~~~~~~~~~~~~~~~~~~~~
	- Protocol: Z-Wave™ (ZM3102N)
	- Frequency Range:
		865.22MHz (ZL7432IN)
		868.42MHz (ZL7432EU)
		869.00MHz (ZL7432RU)
		908.42MHz (ZL7432US)
		916.00MHz (ZL7432IS)
		920.00MHz (ZL7432JP)
		921.42MHz (ZL7432BR)
	- Operating Range: Up to 100 feet line of sight
	- Operating Temp.: -15°C~ 60°C (5°F~140°F)
	- Operating Voltage: 100VAC~240VAC
	- Resistive Load:
		800W for 110VAC
		1300W for 220VAC

.. Inclusion/Exclusion to/from a network
.. ~~~~~~~~~~~~~~~~~~~~~~~
	#. Put controller to Inclusion/Exclusion mode
	#. Turn on and turn off switch that connects with ZL7432 module 4 times. Device will be included/excluded to/from zwave network.
	
	.. image:: ../../images/relay_switch/vision_inwall_micro_2relay_zl7432_d.png
	.. :align: left
	
		
.. Link in Amazon
.. ~~~~~~~~~~~~~~~~~~~~~
	https://www.amazon.com/Vision-Z-Wave-Micro-Switch-relay/dp/B00R883YKU
	
	

.. Configuration description
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Light control 
		- Parameter: 1 (0x01)
		- Size: 1 byte
		- Value:
			1 = To Control Light with 1 Wall Switch & to Control Light With 2 Wall Switches.
			2 = To Control Light with 1 Wall Switch That Has Light Indicator
		- Default: 2
	
	#. Light control 
		- Parameter: 2 (0x02)
		- Size: 1 byte
		- Value:
			1 = With common on/off type switch button used
			2 = With momentary type switch button used.
		- Default: 1
