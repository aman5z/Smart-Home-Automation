https://aman5z.blogspot.com/2024/09/projects.html

Room #1: 

Back in 2021, I have implemented an automation system using an 8-channel relay, a NodeMCU ESP8266, and an AC to DC 5V 2A adapter board, all neatly housed inside a large box. This setup is connected to the tube lights, ceiling fan, Philips Wiz smart LED Bulb (10W), DIY RGB lamp (RGB Strip, ESP8266), study lamp, and three 2-pin sockets, which I use to plug devices like phone chargers and laptops. I've automated these sockets to turn off at a specific time when the device reaches 100% charge, ensuring devices don't overcharge, which is safer. I can safely leave them plugged in overnight without worrying about overcharging!

For AC control, I use a Homemate Wi-Fi IR remote (I tried DIY in past, not reliable and its limited), which allows me to turn the AC on/off, change modes, set the temperature, and more, either via its app or with voice commands through Alexa and Google Assistant. I've also automated the AC to maintain a temperature of 24°C until 3 AM, then increase to 26°C until 5 AM before turning off. The fan is programmed to turn off at 6 AM, helping me wake up on time while saving power. The lights can also be automated to turn on during this schedule, but I’ve left this option as a backup.

Additionally, I've repurposed an old POCO M3 phone that was damaged after a fall (it had a faulty charging port, non-functional SIM card detection, broken flashlight, and GPS). I replaced the display, and only Wi-Fi and Bluetooth work now. To make this more useful, I placed the phone inside a custom holder with an inbuilt 5W speaker and connected it to a 10,000 mAh power bank for extended battery life. The power button was extended externally for easy access. I then removed about 85-90% of the pre-installed bloatware from MIUI, keeping only the essential components, transforming the device into a Smart Home Display similar to an Amazon Echo Show. I use it as my personal, portable voice assistant to control home devices and play music. The device can also be controlled through the Alexa app on my WearOS, making it feel even more futuristic!

Room #2: 

This room is equipped with a Philips Wiz smart LED Bulb (10W), which is used both as a normal light and a night lamp (lighting at just 10% brightness in night mode). I've connected a 40A Solid State Relay (SSR) and a NodeMCU ESP8266 inside the AC stabilizer to control the AC unit's power. I’ve also created a DIY SSR relay using a 3W LED and Light Dependent Resistor (LDR) to manage the AC control via the stabilizer. The ESP8266 inside the stabilizer is programmed with Tasmota, allowing control via an app or through Alexa/Google Assistant. I've automated the AC to turn on until 5 AM, after which the unit turns off, followed by the stabilizer 5 minutes later. This helps me wake up naturally while saving energy. As in Bedroom #1, the light can also be automated to turn on at a specific time, though this feature remains optional. I can also control the system via the Alexa app on my WearOS watch for a futuristic touch!

Living Room:
In the living room, I use an Echo Dot 3rd Gen for voice control. A 4-channel relay, NodeMCU ESP8266, and an AC to DC 5V 1A adapter are housed in a box to manage the connected devices, which include the TV, TV lights (LED strip behind the TV), and 5.1 soundbar home theater system. The devices are integrated with Sinric Pro, which allows for Alexa and Google Assistant compatibility via its app and web dashboard (free for up to 3 devices).

Automation in this room is configured as follows:

When I say, "Alexa, turn on TV," the TV turns on.
When I say, "Alexa, movie time," the TV turns on (if off), the soundbar turns on and connects automatically to the TV via HDMI ARC, TV lights turn on, and the Philips Wiz LED bulb in the living room turns off, creating the perfect movie ambiance.
For "Alexa, movie break," the soundbar (via Homemate Wi-Fi IR remote) pauses the TV/media, and the Wiz light turns on to 50%, allowing for a quick break before resuming the movie.
Everything in the living room is customized using the Alexa app, allowing for seamless control and communication with all connected devices in one place.
Kitchen: 
The kitchen automation includes a water pump motor timer using a 40A SSR and an Arduino Nano. I programmed the timer using simple Arduino code with 3 buttons: a 2-minute option (when unsure about the water tank level), a 7-minute option (when the tank is empty and needs to be filled), and a reset button to stop the pump or change the timer. The setup is powered by an AC to DC 5V 1A adapter and housed in a 2-module electrical box, wired to the existing motor switch. This system ensures efficient water usage, preventing overflows and saving energy. I can also connect a NodeMCU ESP8266 to enable control via a mobile app, Alexa, or Google Assistant from anywhere, but in this case its not necessary.
