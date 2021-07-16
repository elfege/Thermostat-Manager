# Thermostat-Manager: the app that learns from your inputs and gets better over time. 
This app allows you to manage a thermostat settings in many ways. It will learn from your input and get more efficient over time. 

Among many other features, you will be able to: 

1) Set contact sensors rules for both windows (to save power when windows are open) and inside doors (to coordinate with other thermostats states). 
2) Push a button to signal the app that you want your sleeping settings to be on. 
3) Control some windows (with switch capability) and have them opened, weather permitting, in order to avoid overusing your Air Conditionner. 
4) Use a virtual dimmer that will serve as a desired temperature reference. Mostly, this is where the app learns from your inputs, even though it'll also learn from some inputs made on your thermostat directly. However, alexa can't adjust a setpoint on a thermostat that is set to "off", which is a bummer. This is why this also facilitates voice commands with Alexa or Google Home, even when your thermostat is set to off. 
5) You can also use the intelligent automatic evaluation of your needs (you will still need a virtual dimmer): let the app set everything for you. This algorithm is meant to optimize both power saving and comfort, but it can also be customized with maxima and minima inputs in settings. 
6) Use a switch to control a heater, another switch to control a cooler to add more power during polar vortex or heat waves. You can set the extra heater to be triggered only when it's really too cold outside.
7) If your alternate heater is connected to a switch with power capability, the app will offer you to use this capability to select a total max power consumption and an order of priority under certain weather conditions: keep power consumption under control. 
8) Use a power meter to assert your HVAC good operation (consistency between power consuption and desired state) so the app can try to send commands again (usefull under bad mesh conditions using Z-wave 1.0 thermostats). 
9) Several air circulation options will allow you to optimize air distribution in your home when the thermostat is cooling. 


NB: You'll need to have a weather station or a temperature sensor located outside your home.

**Updates July 2021 :** 

Improved Celsius management. I still need feedback on this from those who might use Celsius as it would be very impractical for me to test it in my home. 

I added some simple but nonetheless powerful elements of A.I., with more to come in a near future. If you chose the full "auto" method, the app will progressively implement a map of your preferences each time you change your target temperature/ cooling or heating setpoint; it will then remember them to approximate your preferences under similar circumstances when they occur. 

For now the app learns based on outside temp and a basic preset map that gets implemented over time. In the future I'll implement more parameters, such as differentiated humidity values ([[inside humidity, outside humidity, outside temperature] : target amplitude]]), which will allow the app to be more thorough. 

Note that these features are already available with the app called "A.I. Thermostat manager" and supposed to work in parallel with "Thermostat Manager", using the dimmer to share computed results. However, this is an old workaround that takes too much ressources anyway so it is to be entirely reworked and implemented into Thermostat Manager directly, as I have started doing so with this new learning algorithm. In order to achieve complete learning abilities, I'll probably use the new file feature in Hubitat to store the "big data" needed to that effect.
