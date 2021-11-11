# CRYSTAL VISION HUD
### Head-Up Display (HUD) System for safe driving

#### Attention: This repository does not contain diagrams and drawings of projector optics.


Crystal Vision is a portable Head-Up Display (HUD) system that projects an image on the windshield of your car. 
Both the driver and the passengers see it as a semi-transparent image that “levitates” over the hood of the car.

#### Copyright (C) 2015-2018, Crystal Vision Ltd.


https://user-images.githubusercontent.com/49099551/141296656-99a9382b-fc6b-408f-bb68-5c6743e9c2cb.mp4


## VISUAL CHARACTERISTICS

* Resolution: 854 x 480
* Perceived distance: 1.8-2.2 meters (depends on winshield geometry)
* Size: 17"
* Frequency: 60 Hz
* Color coverage:  ~70% sRGB
* Brightness: 1150 cd/m² (only for visible parts)
* Proprietary Remote Canvas technology



## TECHNICAL SPECIFICATIONS

* CPU: Allwinner H6 Quad-Core 64-bit Cortex-A53 @ 1.8GHz
* RAM: LPDDR3 2Gb @ 533Mhz
* ROM: 32Gb TF/MMC
* Power supply: DC 12V, 1.2A (max)
* Interfaces: IEEE 802.11 b/g/n (WiFi), Bluetooth 5.1, USB 2.0, OBDII
* Control OS: Android 9.0 Pie
* Dimensions: 83mm x 52mm x 30mm
* Weight: 115g


## TERMINOLOGY

* Projector - device for displaying projected images in windshield.
* Host phone — the phone on which the manager and client applications are installed.
* Manager - a gateway program through which client applications send graphic messages to the projector.
* Client application - an android application that, using the RemoteCanvas API, draws graphic messages on the projector. 


https://user-images.githubusercontent.com/49099551/141305224-d17a0be4-0d8c-40f3-b766-57251145a1aa.mp4



## DESCRIPTION

The CRYSTAL_HUD_MANAGER module is an android application that is installed on the host phone and acts as a gateway through which applications send messages to the projector.

The CRYSTAL_HUD_MANAGER function as a gateway includes:
* Controlling the concurrent access model of client applications to the projector
* Prioritize access for different applications
* Authorization of client applications.
* Work with three modes: asynchronous messages, synchronous messages, streaming. 


## WEB RESOURCES:

http://crystal-hud.tech Crystal Vision HUD information web site

https://github.com/AdrianTunkin/crystal_vision_hud - GitHub web site hosting the Hardware and Software sources



## LICENSE

### HARDWARE
The Hardware project is released under the Creative Commons Attribution-Share Alike 3.0 United States License.
You may reproduce it for both your own personal use, and for commercial use. 
You will have to provide a link to the original creator of the project http://crystal-hud.tech on any documentation or website.
You may also modify the files, but you must then release them as well under the same terms.
Credit can be attributed through a link to the creator website: http://crystal-hud.tech

### SOFTWARE
The software is released under GPL3.

### DOCUMENTATION
The documentation is released under the Creative Commons Attribution-Share Alike 3.0 United States License.

