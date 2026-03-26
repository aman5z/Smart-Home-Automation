
# 🏠 My DIY IoT & Smart Home Automation Hub

Welcome to my central repository for all my DIY IoT, Smart Home, and hardware automation projects. This repo documents how I've transformed standard household items, appliances, and even my motorcycle into voice-controlled, automated smart devices using ESP8266/ESP32, Arduino, and various custom integrations.

## 📋 Table of Contents
- [Room #1: The Ultimate Smart Bedroom & Custom Smart Display](#room-1-the-ultimate-smart-bedroom--custom-smart-display)
- [Room #2: Automated AC & Natural Wake-up System](#room-2-automated-ac--natural-wake-up-system)
- [Living Room: Voice-Controlled Home Theater Setup](#living-room-voice-controlled-home-theater-setup)
- [Kitchen: Smart Water Pump Timer](#kitchen-smart-water-pump-timer)
- [Smart Extension Box V3](#smart-extension-box-v3)
- [Bike Keyless Entry via IoT](#bike-keyless-entry-via-iot)
- [IoT RC Car with Custom Web Controller](#iot-rc-car-with-custom-web-controller)

---

## 🛏️ Room #1: The Ultimate Smart Bedroom & Custom Smart Display

### Features & Automations:
* **Smart Charging Sockets:** 3x 2-pin sockets programmed to cut power at a specific time when devices (phones/laptops) reach 100% charge, preventing overnight battery degradation.
* **Automated AC Routine:** Uses a Homemate Wi-Fi IR remote to maintain 24°C until 3 AM, bumps up to 26°C until 5 AM, and then turns off.
* **Smart Lighting & Fan:** Automated ceiling fan turns off at 6 AM to help me wake up on time. Philips Wiz LED (10W), DIY RGB strip lamp, and study lamp are all integrated.
* **DIY Smart Display (Repurposed POCO M3):** Salvaged a broken phone (no charging port, SIM, or GPS). Replaced the display, added an inbuilt 5W speaker, and connected a 10,000 mAh power bank. Stripped 90% of MIUI bloatware to turn it into a dedicated, portable Alexa/Google Assistant hub. 

**Hardware:** NodeMCU ESP8266, 8-Channel Relay, 5V 2A AC-DC Adapter, Homemate Wi-Fi IR Remote, Repurposed Android Phone.

<details>
<summary>📸 View Gallery</summary>
<br>

![IMG_20210604_180912](https://github.com/user-attachments/assets/d0be9eba-0ef4-4f32-98a3-0c69c008b71e)
![IMG_20190227_131145](https://github.com/user-attachments/assets/237e2b13-2264-42ed-a0b6-254da94fd6bf)
![IMG_20210626_004008](https://github.com/user-attachments/assets/8561c240-72d6-4f1b-ba6d-18d6fc92f8fe)
</details>

---

## 🌙 Room #2: Automated AC & Natural Wake-up System

### Features & Automations:
* **Night Mode Lighting:** Philips Wiz smart LED Bulb programmed to drop to 10% brightness at night.
* **Integrated AC Stabilizer Control:** Built an ESP8266 directly into the AC stabilizer. Paired with a DIY SSR relay (using a 3W LED and LDR) to manage power safely. 
* **Tasmota Integration:** Flashed with Tasmota for local and cloud control via Alexa/Google Assistant and WearOS.
* **Sleep Routine:** AC runs until 5 AM, then shuts off. The stabilizer automatically cuts power 5 minutes later, saving energy and allowing for a natural wake-up.

**Hardware:** NodeMCU ESP8266 (Tasmota), 40A Solid State Relay (SSR), LDR, 3W LED.

<details>
<summary>📸 View Gallery</summary>
<br>

![IMG-20190306-WA0002](https://github.com/user-attachments/assets/8b1e92be-25d1-401c-bfc4-19262e979fd0)
![IMG_20210311_004233](https://github.com/user-attachments/assets/c6bcff7f-ae99-41e4-95b8-08805f890211)
![IMG_20210224_010514](https://github.com/user-attachments/assets/e158ecc4-8f6c-4edc-9e2f-aad308c6d415)
</details>

---

## 📺 Living Room: Voice-Controlled Home Theater Setup

### Features & Automations:
Powered by Sinric Pro, everything is synced seamlessly with Alexa routines:
* *"Alexa, turn on TV"* -> Powers up the display.
* *"Alexa, movie time"* -> TV turns on, Soundbar powers up (auto-connects via HDMI ARC), LED bias lighting turns on, and room lights turn off for a theater experience.
* *"Alexa, movie break"* -> Soundbar pauses media, and room lights raise to 50% brightness.

**Hardware:** Echo Dot 3rd Gen, NodeMCU ESP8266, 4-Channel Relay, 5V 1A Adapter, Sinric Pro.

<details>
<summary>📸 View Gallery</summary>
<br>

![IMG_4515](https://github.com/user-attachments/assets/5412da56-6eb3-4dc0-8d80-d5d6e2724ce1)
![IMG_3498](https://github.com/user-attachments/assets/4e0b77b3-6078-4687-a82e-5426b22235b0)
![IMG_20210213_175929](https://github.com/user-attachments/assets/e12c7b9d-530f-4d54-9828-e7b2d4534518)
</details>

---

## 💧 Kitchen: Smart Water Pump Timer

### Features & Automations:
A purely functional, offline-first approach to water management. Housed in a standard 2-module electrical box and wired to the existing switch.
* **Manual Timer Logic:** Includes 3 physical buttons:
  * **2-Minute Mode:** Quick top-up when tank levels are unknown.
  * **7-Minute Mode:** Full fill for an empty tank.
  * **Reset:** Instantly stop the pump or change modes.
* Prevents water overflow and saves electricity.

**Hardware:** Arduino Nano, 40A SSR, 5V 1A Adapter. *(ESP8266 ready, but kept offline for simplicity and reliability).*

<details>
<summary>📸 View Gallery</summary>
<br>

![IMG-20190306-WA0002](https://github.com/user-attachments/assets/8d6a2c53-3220-46e5-84d7-4cf4a011ea59)
![IMG-20190306-WA0000](https://github.com/user-attachments/assets/23a01407-c903-4636-97c8-b50a0d334327)
![IMG_20210308_233706](https://github.com/user-attachments/assets/4dfeeca6-89dc-4a79-9e3e-35f5955ab0f1)
![IMG_20210213_175929](https://github.com/user-attachments/assets/99f304e5-de93-49ae-a8ba-3ad4013386cd)
</details>

---

## 🔌 Smart Extension Box V3

### Features & Automations:
Upgraded a standard GoldMedal 6-socket extension board (which originally had only one master switch) into an individually addressable smart power strip.
* **Individual Control:** All 6 sockets can be controlled independently via ESP RainMaker, Alexa, or Google Assistant.
* **IR Remote Integration:** Added a TSOP receiver. Mapped a generic IR remote to toggle individual sockets, with a master '0' button to kill all power.
* **Developer Friendly:** Built-in external USB-A port and reset switch so the ESP32 can be flashed via Arduino IDE without opening the casing.

**Hardware:** ESP32 Dev Board, 6-Channel Relay (4+2), IR Receiver (TSOP), 5V 2A Adapter.

<details>
<summary>📸 View Gallery</summary>
<br>

![IMG_3516(1)](https://github.com/user-attachments/assets/cac47e85-987c-4a39-9a94-53f3c51ccb8f)
![IMG_3524(1)](https://github.com/user-attachments/assets/54b86a8e-9bea-4ef4-89e0-3bc726256ef4)
![IMG_3518(1)](https://github.com/user-attachments/assets/5bd905b8-b556-4512-ae0d-0466f648557f)
</details>

---

## 🏍️ Bike-Keyless-Entry-via-IoT

### Features & Automations:
Transformed a standard motorcycle into a fully keyless, voice-controlled vehicle!
* **IoT Ignition Control:** Controls ignition, kill switch, and self-start. Connects to phone hotspot (matching home SSID) to grant internet access on the go.
* **Proximity Lock/Unlock:** Integrated an old RC Car RF module into a keychain. The bike automatically unlocks when I approach and locks when I walk >10 meters away.
* **"Tony Stark" Helmet Start:** DIY Bluetooth receiver in my helmet allows me to start the engine directly from the helmet.
* **WearOS Integration:** Start the bike using the Alexa app right from my smartwatch.

**Hardware:** NodeMCU ESP8266, 4-Channel Relay, 12V to USB Charger, RF Module, Sinric Pro.

<details>
<summary>📸 View Gallery</summary>
<br>

![IMG_20190227_012850](https://github.com/user-attachments/assets/358f6cf6-d342-41a7-b6e9-23ce1a5e5a14)
![IMG_20210406_165326](https://github.com/user-attachments/assets/e9c187cd-d016-4156-8f96-107bf1c1bccc)
![IMG_20210404_184812](https://github.com/user-attachments/assets/f7efff28-c176-4323-afb8-589dcb54dfca)
![IMG_20210404_152327](https://github.com/user-attachments/assets/ae0b3608-02f8-418a-86fc-22fe585ec64e)
</details>

---

## 🏎️ IoT RC Car with Custom Web Controller

### Features & Automations:
A completely DIY Wi-Fi controlled car built from recycled electronic junk.
* **Locally Hosted:** The ESP8266 acts as an Access Point/Web Server serving a custom HTML/JS control page. No external apps required—just connect to the Wi-Fi and open the browser.
* **Recycled Tech:** Chassis, gearbox, motors, and wheels were entirely salvaged from broken toys.

**Hardware:** NodeMCU ESP8266, L298N (or similar) Motor Controller, Salvaged RC Parts.

<details>
<summary>📸 View Gallery</summary>
<br>

![IMG_20190320_020957](https://github.com/user-attachments/assets/baee22df-9cd6-421b-a719-ea115f030670)
![IMG_20190309_094614](https://github.com/user-attachments/assets/645bb752-4d5c-4964-a1c4-3da03b0684cd)
![IMG_20190320_021026](https://github.com/user-attachments/assets/d6736664-087f-496b-b023-b16bc1a70720)
</details>

---
*Built with 💻 and ☕ by aman5z.in
