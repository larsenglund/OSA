# What is this?
A series of open smart automation devices and software. All devices support WiFi and mesh networking and use open standards such as MQTT for communication. Works with Google Home and Alexa. Easy creation of automation rules, scheduling and scenes.

# Devices
Available devices are (in no particular order)
* [LD (LED Dimmer)](#ld-led-dimmer)
* [ED (Embedded Dimmer)](#ed-embedded-dimmer)
* [WD (Wall Dimmer)](#wd-wall-dimmer)
* [ET (Embedded Thermostat)](#et-embedded-thermostat)
* [WT (Wall Thermostat)](#wt-wall-thermostat)
* [WS (Wall Sensor)](#ws-wall-sensor)
* [RC (Remote Control)](#rc-remote-control)

## LD (LED Dimmer)
LED controller with two dimmer channels and two RGB channels.
The dimmer channels are for controlling any type of LED that uses 5-30VDC with a max total current of 10A (120W @ 12V or 240W @ 24V).
The RGB channels are for controlling addressable RGB LED strips.

<bild på; schematic, pcb (eller gerber), populerat pcb, inkapsling (fusion360-render + foto), i drift i hemmiljö>

## ED (Embedded Dimmer)
Dimmer with two channels for embedding in junction boxes. Accepts 90-264VAC with a max total load of 800W or a max current of 4A.
Features trailing edge dimming that eliminates the noise and current spikes that are common with common leading edge dimmers.
Features over voltage, over current and over temperature protection.
Adapted to the global 55x55mm platform and compatible with Schneider Exxact and similar 55x55mm systems.
Can be embedded behind regular switches and outlets and use the existing switches to control the dimmers but is recommended to be combined with the WD (Wall Dimmer) insert.
Can be used without the dimming component to simply make regular switches wireless or replace them with a WD (Wall Dimmer) insert.

<bild på; schematic, pcb (eller gerber), populerat pcb, inkapsling (fusion360-render + foto), i drift i hemmiljö>

## WD (Wall Dimmer)
Insert with a 1.44 inch full color display, 9 tactile switches and optional temperature sensor.
Adapted to the global 55x55mm platform and compatible with Schneider Exxact and similar 55x55mm systems.

<bild på; schematic, pcb (eller gerber), populerat pcb, inkapsling (fusion360-render + foto), i drift i hemmiljö>

## ET (Embedded Thermostat)
Thermostat for under floor heating. Connections for floor temperature sensor and one heat cable.
Heat cable max current is 16A.
Floor temperature sensor should be NTC 10K (adaptable from 1K to 100K).
Features over voltage, over current and over temperature protection.

<bild på; schematic, pcb (eller gerber), populerat pcb, inkapsling (fusion360-render + foto), i drift i hemmiljö>

## WT (Wall Thermostat)
Insert with a 1.44 inch (128x128 pixels) full color display, 9 tactile switches and temperature sensor.
Adapted to the global 55x55mm platform and compatible with Schneider Exxact and similar 55x55mm systems.

<bild på; schematic, pcb (eller gerber), populerat pcb, inkapsling (fusion360-render + foto), i drift i hemmiljö>

## WS (Wall Sensor)
Wall or ceiling mounted sensor that measure;
* Temperature (°C/°F)
* Humidity (%RH)
* Light (lux)
* Pressure (hPa)
* Sound Pressure Level / Noise (dB SPL)
* Volatile Organic Compounds (VOC)
* Carbon Dioxide (CO<sup>2</sup>)
* Particulate Matter (PM<sub>10</sub>/PM<sub>2.5</sub>)

Also features;
* Optical smoke detector
* Piezo siren for alarms
* RGB led
* Battery backup (lipo + charger)

<In WS more-info-page, link to CO2 studies: http://vair-monitor.com/2016/09/29/sleeping-closed-room-indoor-co2-analyze/>

<bild på; schematic, pcb (eller gerber), populerat pcb, inkapsling (fusion360-render + foto), i drift i hemmiljö>

## RC (Remote Control)
Handheld remote control with 1.44 inch (128x128 pixels) full color display and 12 tactical buttons.
Uses the very common (and thus economic) Nokia BL-5C battery with up to 208 days battery time.
USB rechargeable with standard mini USB phone charger.

<bild på; schematic, pcb (eller gerber), populerat pcb, inkapsling (fusion360-render + foto), i drift i hemmiljö>

# Software
## OSA configurator
Mobile phone app that automatically finds and configures all devices.
<bild på; app på telefonen + kort film?>

## Server
Optional local server that allows automation and data collection to be kept local and private.
Raspberry Pi with Homeassistant and additional software.
<bild på; GUI:n (HADashboard på väggpadda, på mobilen, etc), servern i inkapsling (pi3 i standardlåda?)>

# Background
The project was born from frustration with bad offline dimmers and environmental sensors with non-intuitive interfaces and one way communication that often fails, and a feeling that the comercial options avalable where to expensive and restricted.
