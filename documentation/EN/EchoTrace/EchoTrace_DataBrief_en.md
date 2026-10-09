[Main](/) ❯ [Navigation & tracking systems](/navigation_and_tracking_systems_en) ❯ **EchoTrace: Data brief**

<div style="page-break-after: always;"></div>

| ![Trackdyne](/documentation/logo.svg) | ![EchoTrace_Pack](/documentation/echotrace_pack_small.png) |
| :---: | ---: |
| [trackdyne.com](https://trackdyne.com/) <br/> [support@trackdyne.com](mailto:support@trackdyne.com) | **EchoTrace** - Underwater tracking system <br/> Data brief |

<div style="page-break-after: always;"></div>

## General information
The **EchoTrace** system is **the easiest to use** and at the same time accurate solution for tracking underwater objects. The system **does not require any calibration** and integration: it is enough to place an autonomous pinger beacon [EchoTrace Pinger](EchoTrace_Pinger_Specification_en.md) on an underwater object (ROV, AUV, diver, etc.), and four navigation buoys on the surface of the water [EchoTrace GIB](EchoTrace_GIB_Specification_en.md). This configuration allows the user to monitor in real time the movement of an underwater object in 3D: absolute geographic coordinates + depth.
A distinctive feature of the system is the ability to work with diver's wireless telephone [SubVox Diver](/documentation/EN/SubVox/SubVox_Diver_Specification_en.html) as a pinger, thus combining two-way voice communications and navigation.

When working with a pinger, the navigation receiver [EchoTrace RF Dongle](EchoTrace_RF_Dongle_Specification_en.md) emulates the protocol of conventional GNSS receivers, and it can be connected to any software that supports displaying the position of a GNSS receiver on the map. For example, GoogleEarth, SAS.Planet, etc.
<div style="page-break-after: always;"></div>

## System composition

|  |  |
| :---: | :--- |
| ![EchoTrace GIB](/documentation/echotrace_gib_h_small.png) | [EchoTrace GIB](EchoTrace_GIB_Specification_en.md) <br/> GNSS-equipped sonobuoy |
| ![EchoTrace Pinger](/documentation/dev_big_wbat_li_small.png) | [EchoTrace Pinger](EchoTrace_Pinger_Specification_en.md) <br/> Pinger-beacon |
| ![EchoTrace RF dongle](/documentation/echotrace_rf_dongle.png) | [EchoTrace RF Dongle](EchoTrace_RF_Dongle_Specification_en.md) <br/> Navigation receiver/RF dongle |

The minimum set includes four sonobuoys [EchoTrace GIB](EchoTrace_GIB_Specification_en.md) and one transmitting device, depending on the user task:
* If it is necessary to provide the diver with navigation data simultaneously with voice communication, then a diver's wireless telephone [SubVox Diver](/documentation/EN/SubVox/SubVox_Diver_Specification_en.html) is used; In this case, the diver's geoposition will be determined at the moment when he releases the PTT button, i.e. ends the transmission of a voice message;
* If it is necessary to determine the location of a remotely controlled vehicle (ROV) or a diver without the need to use voice communication, then a pinger beacon [EchoTrace Pinger](EchoTrace_Pinger_Specification_en.md) is used. The pinger works autonomously and the geoposition of the object on which the pinger is attached will be updated every two seconds.

### When working with pinger

It is enough to simply connect the navigation receiver to any card plotter that supports [NMEA0183 RMC and GGA](EchoTrace_RF_Dongle_Protocol_Specification_en.md) messages. In this option, the user has access to:
- geographic location of the object on which the pinger is attached
- course of movement of the object

When using the EchoTrace host application (available on request from [support@trackdyne.com](mailto:support@trackdyne.com)), the following additionally become available:
- positions of navigation buoys and charge of their built-in power sources;
- course and range to the reference point, for which the user can select one of four buoys, the built-in navigation receiver [EchoTrace RF Dongle](EchoTrace_RF_Dongle_Specification_en.md) or a point with an arbitrarily specified coordinate;
- water temperature & depth;
- pinger supply voltage;

### When working with SubVox Diver wireless diver's telephone

Requires the diver tracking application (available on request from [support@trackdyne.com](mailto:support@trackdyne.com)). In this case, the user has access to the positions of up to 255 divers, determined at the end of each voice transmission from the diver.


<div style="page-break-after: always;"></div>

## Solved problems
* Monitoring the position of an underwater object (divers, ROVs, AUVs, etc.);
* Determining the course of movement of an underwater object;
* Assistance in driving an underwater object to a surface control point and back;

<div style="page-break-after: always;"></div>

## Distinctive features
* Work in absolute geographical coordinates;
* A floating base of four sonobuoys allows you to monitor both the pinger [EchoTrace Pinger](EchoTrace_Pinger_Specification_en.md) and the diving telephone exchange [SubVox Diver](/documentation/EN/SubVox/SubVox_Diver_Specification_en.html);
* No preliminary configuration and calibration of the system and its components is required;
* No information connection between the object and the pinger is required - the pinger is mechanically attached to the underwater carrier;
* Transferring the calculated position of an underwater object to third-party software via a serial port using the NMEA0183 protocol;
* Recording the movement track of an underwater object;

<div style="page-break-after: always;"></div>

## Geometric limitations
* _From each to each of the buoys there should be no more than 1500 meters and no less than 30 meters_
* _The buoys should be arranged in a convex quadrangle so that its sides are approximately equal and differ by no more than 2 times_
* _The maximum diving depth of the pinger should not exceed the dimensions of the navigation base_
* _The greatest accuracy of the system is achieved within the buoy figure, and work should always begin within this figure. Exiting the figure is possible, but the accuracy may decrease significantly as the positioned object moves away from the buoy figure_

<div style="page-break-after: always;"></div>

_________  

