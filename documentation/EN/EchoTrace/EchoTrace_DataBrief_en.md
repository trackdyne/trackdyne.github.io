[Main](/) ❯ [Navigation & tracking systems](/navigation_and_tracking_systems_en.html) ❯ **EchoTrace: Data brief**

<div style="page-break-after: always;"></div>

| ![Trackdyne](/documentation/logo.svg) | ![EchoTrace_Pack](/documentation/echotrace_pack_small.png) |
| :---: | ---: |
| [trackdyne.com](https://trackdyne.com/) <br/> [support@trackdyne.com](mailto:support@trackdyne.com) | **EchoTrace**<br/> Data brief |

<div style="page-break-after: always;"></div>

## General information
The **EchoTrace** system is **the easiest to use** while also providing an accurate solution for tracking an underwater object. The system **does not require any calibration** or integration: simply attach an autonomous [EchoTrace Pinger](/documentation/EN/EchoTrace/EchoTrace_Pinger_Specification_en.html) pinger beacon to an underwater object (ROV, AUV, diver, etc.) and place four [EchoTrace GIB](/documentation/EN/EchoTrace/EchoTrace_GIB_Specification_en.html) navigation buoys on the water surface. This configuration allows the movement of an underwater object to be tracked in real time in 3D: absolute geographic coordinates + depth.
A distinctive feature of the system is its ability to use [SubVox Diver](/documentation/EN/SubVox/SubVox_Diver_Specification_en.html) diver telephone stations as pingers, thus combining two-way voice communication and navigation.

When used with a pinger, the [EchoTrace RF Dongle](/documentation/EN/EchoTrace/EchoTrace_RF_Dongle_Specification_en.html) navigation receiver emulates the protocol of conventional GNSS receivers and can be connected to any software that supports displaying the position of a GNSS receiver on a map, such as Google Earth, SAS.Planet, etc.

<div style="page-break-after: always;"></div>

## System composition

|  |  |
| :---: | :--- |
| ![EchoTrace GIB](/documentation/echotrace_gib_h_small.png) | [EchoTrace GIB](/documentation/EN/EchoTrace/EchoTrace_GIB_Specification_en.html) <br/> Navigation sonobuoy (receiver) |
| ![EchoTrace Pinger](/documentation/dev_big_wbat_li_small.png) | [EchoTrace Pinger](/documentation/EN/EchoTrace/EchoTrace_Pinger_Specification_en.html) <br/> Pinger beacon |
| ![EchoTrace RF dongle](/documentation/echotrace_rf_dongle.png) | [EchoTrace RF Dongle](/documentation/EN/EchoTrace/EchoTrace_RF_Dongle_Specification_en.html) <br/> Digital radio receiver |

The minimum system configuration includes four [EchoTrace GIB](/documentation/EN/EchoTrace/EchoTrace_GIB_Specification_en.html) sonobuoys and one transmitting device, depending on the user's task:
* If a diver needs navigation data along with voice communication, a [SubVox Diver](/documentation/EN/SubVox/SubVox_Diver_Specification_en.html) diver telephone station is used. In this case, the diver's position is determined when they release the PTT button, i.e., finish transmitting a voice message;
* If the position of a remotely operated vehicle (ROV) or a diver needs to be determined without voice communication, an [EchoTrace Pinger](/documentation/EN/EchoTrace/EchoTrace_Pinger_Specification_en.html) pinger beacon is used. The pinger operates autonomously, and the position of the object to which it is attached is updated every two seconds.

### When used with a pinger

Simply connect the navigation receiver to any chartplotter that supports [NMEA0183 RMC and GGA](/documentation/EN/EchoTrace/EchoTrace_RF_Dongle_Protocol_Specification_en.html) messages. In this configuration, the user has access to:
- the geographic position of the object to which the pinger is attached
- the object's course of movement

### When used with SubVox Diver diver stations

[SubVox Diver](/documentation/EN/SubVox/SubVox_Diver_Specification_en.html) stations can emit a navigation signal at the end of each voice transmission. The buoy measurements must be processed by an external host system to calculate the diver's position. Assign a unique address to each diver station.

<div style="page-break-after: always;"></div>

## Tasks to be solved
* Tracking the position of an underwater object in real time (divers, ROVs, AUVs, etc.);
* Determining the course of movement of an underwater object;
* Assistance in guiding an underwater object to a surface control point, and vice versa;

<div style="page-break-after: always;"></div>

## Distinctive features
* Operation in absolute geographic coordinates;
* A floating base of four sonobuoys allows tracking of both an [EchoTrace Pinger](/documentation/EN/EchoTrace/EchoTrace_Pinger_Specification_en.html) pinger and a [SubVox Diver](/documentation/EN/SubVox/SubVox_Diver_Specification_en.html) diver telephone station;
* No preliminary setup or calibration of the system or its components is required;
* No data interface is required between the object and the pinger: the pinger is mechanically attached to the underwater carrier;
* Transfer of the calculated position of an underwater object to third-party software via a serial port using the NMEA0183 protocol;
* Recording the movement track of an underwater object;

<div style="page-break-after: always;"></div>

## Geometric limitations
* _The distance between any two buoys must be no more than 1500 meters and no less than 30 meters_
* _The buoys must be arranged in a convex quadrilateral so that its sides are approximately equal and differ by no more than a factor of 2_
* _The maximum diving depth of the pinger must not exceed the dimensions of the navigation base_
* _The greatest system accuracy is achieved within the polygon formed by the buoys, and operation must always begin within this polygon. Operation outside the polygon is possible, but accuracy may decrease significantly as the object being positioned moves away from the buoy polygon_

<div style="page-break-after: always;"></div>

_________
