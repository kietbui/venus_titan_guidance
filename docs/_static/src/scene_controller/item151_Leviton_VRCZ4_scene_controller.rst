Leviton Z-Wave VRCZ4-M0Z 4-Button In-Wall Scene Controller
---------------------------------

	.. image:: ../../images/scene_controller/Leviton_scene_controller.jpg
	.. :align: left
	
Product Description
~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Ideal for remote control of up to four different zones/areas.
	#. Each button on a RF controller can be associated with up to 32 select Z-Wave compatible devices in a system area.
	#. LED illuminates when the controlled scene is active or when one load is on in any zone or area.
	#. High gloss finish complements a wide range of décors.
	#. Neutral required: yes
	#. May be used as a repeater or range extender

Working with PhD
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. Control your Leviton 4-Button Scene Controller and other connected devices with the Zinno app available on iOS&Android
	#. With PhD, you can activate the scences that associated with 4 button on Leviton Scene Controller by the Zinno App or voice commands (Google Assistant or Amazon Alexa)

Add Leviton 4-Button Scene Controller to PhD's network
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
	#. On the Zinno app, press Left Menu Bar, then select “Devices”
	#. Select “+” button to put the PhD in inclusion mode, keep the Leviton Scene Controller close to PhD within 10 feet (3 meters)
	#. Press the left side of 1st and 3rd buttons
	#. If detecting a new device successfully, PhD will announce message “Found Device”, and on the Zinno app will display the dialog box, asking user to interact with device one more time
	#. Press and hold the left side of 1st and 3rd buttons. Wait 5 seconds until the Leviton LED turns Amber. Release the buttons and the Leviton LED will blink Amber. You are now in Programming mode. PhD will announce message “The device is being added”
	#. If adding the relay successfully, PhD will announce “Adding Leviton 4-Button Scene Controller success” and on Zinno app will display the dialog boxes that indicate user has added device successfully	

	.. image:: ../../images/scene_controller/Leviton_scene_controller_d.jpg
	.. :align: left

Specification
~~~~~~~~~~~~~~~~~~~~~~
	- Model number: 				VRCZ4-M0Z
	- Power source: 				Wall-Powered, 120VAC, 60Hz
	- Protocol: 					Z-Wave
	- Dimension:					4.13 x 1.75 x 1.68 inches
..	- Weight:						0.1 pounds
	- Color: 						White/Ivory/Light Almond
	
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
