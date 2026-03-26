
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

![IMG-20190306-WA0000](https://github.com/user-attachments/assets/c741b377-163f-420e-9a08-03da34a4cbe1)
![IMG_20210626_004008](https://github.com/user-attachments/assets/fb8143f0-f338-4ef6-b7a9-329f63ccce7b)
![IMG_20210604_180912](https://github.com/user-attachments/assets/eba33c03-7e59-4e0f-8084-dab73e180ccc)
![IMG_20210311_004233](https://github.com/user-attachments/assets/5efd6039-7ff8-47de-94d5-cde6d0406344)
![IMG_20210308_233706](https://github.com/user-attachments/assets/eebd3ba9-b88d-48d7-b955-996f65cf0dae)
![IMG_20210224_010514](https://github.com/user-attachments/assets/864e2ac0-0ec4-4348-ad3f-90b6f47e9557)
![IMG_20210213_175929](https://github.com/user-attachments/assets/d0138cf2-5a32-4a73-a4dd-88968814c742)
![IMG_20190227_131145](https://github.com/user-attachments/assets/3dbbb0d9-d3af-4a27-9ea4-1380a3551511)
![IMG_4515](https://github.com/user-attachments/assets/b2539fcc-647c-4372-a9e3-a6c5f4065909)
![IMG_3498](https://github.com/user-attachments/assets/12ed73f1-18b6-4051-b777-5e059530f31e)
![IMG-20210625-WA0012](https://github.com/user-attachments/assets/618cadc4-40b2-4204-8423-cb07b166946a)
![IMG-20210619-WA0012](https://github.com/user-attachments/assets/02cf26b4-37cf-4695-a2cd-d76c7a91f2b2)
![IMG-20190306-WA0002](https://github.com/user-attachments/assets/67e2337d-2c52-4687-a8e1-94d22755feb4)
![IMG-20190306-WA0001](https://github.com/user-attachments/assets/8e6aa2b3-8c52-42bf-903e-7f368c8b47ac)



Smart Extension Box V3 

![MixCollage-07-Mar-2026-04-04-AM-459](https://github.com/user-attachments/assets/774dc208-1f0b-446a-a102-5dea3f74b8d3)
![IMG_3524(1)](https://github.com/user-attachments/assets/6cadf5c0-129d-4a31-b041-b7aa7742c88e)
![IMG_3518(1)](https://github.com/user-attachments/assets/ce578bfb-d1e8-44d5-b606-efb4e546028f)
![IMG_3516(1)](https://github.com/user-attachments/assets/71806ac6-8ac4-4aa4-8562-5d0d89059940)



 Smart Extension Box V3 For this project, I used a GoldMedal brand extension box with 6 x 3-pin sockets. Originally, it had a single switch to control all the sockets at once. I upgraded it using a 4-channel + 2-channel=6 channel relay, an ESP32 dev board, and an AC to DC 5V 2A adapter. I added a reset switch, a USB-A port for reprogramming the device via Arduino IDE, and an external port to avoid opening the box each time.

The extension box now has individual control switches thanks to an IR receiver module (TSOP) and a small generic IR remote. I extracted the IR values and assigned them to each of the six sockets, using the '0' button to turn off all sockets at once. The box can also be controlled via the ESP RainMaker app, Alexa, or Google Assistant, allowing for timers and automation.




# Bike-Keyless-Entry-via-IoT

![IMG_20210404_184812](https://github.com/user-attachments/assets/e7a24218-40b1-4f31-ab70-6d3c51646aad)
![IMG_20210404_152327](https://github.com/user-attachments/assets/aa6e3ae5-88dd-41b2-86d0-458cd19a1b24)
![IMG_20210201_165659](https://github.com/user-attachments/assets/a6bb85e9-b589-4813-bb48-85f87d920ca4)
![IMG_20190227_012850](https://github.com/user-attachments/assets/024972c5-6d55-4a3f-86a8-48cb64a58318)
![IMG_20220214_001356](https://github.com/user-attachments/assets/30563633-3b55-4f2d-984b-d222f8343e9e)
![IMG_20210406_165326](https://github.com/user-attachments/assets/b3ba30cb-2527-42ee-9a87-ac66c5cb82ec)


This project uses a 4-channel relay and a NodeMCU ESP8266, connected via Sinric Pro (which allows for up to 3 devices for free). Power is supplied by a 12V to USB charger connected to the bike's battery (or a power bank can be used). The system is connected to the bike's ignition, kill switch (to turn the engine on/off without turning off the ignition), and self-start switch.
For added fun, I also connected the high beam light switch and horn switch (as a car unlock method), but these are limited due to Sinric Pro’s 3-device limitation. The bike can be controlled via Alexa and Google Assistant. I’ve DIYed a Bluetooth receiver into my helmet, allowing me to turn on the bike while wearing it, giving me a Tony Stark/Iron Man-like experience!

Additionally, I installed an RF module salvaged from an old RC car, which I transformed into a remote keychain. This makes the bike fully keyless—automatically unlocking when I’m near and locking when I move more than 10 meters away. Since I’m usually out and about, I activate my phone’s mobile hotspot (with the same SSID as my home network) to make the system work, although Bluetooth is another option with more limited range.

I can also control the system via the Alexa app on my WearOS watch for a futuristic touch!


