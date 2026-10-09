[Main](/) ❯ [Navigation & tracking systems](/navigation_and_tracking_systems_en) ❯ **VigilArc USBL: Data brief**
<div style="page-break-after: always;"></div>

| ![Trackdyne](/documentation/logo.svg) | ![logo](/documentation/vigilarc_package.png) |
| :---: | ---: |
| [trackdyne.com](https://trackdyne.com/) <br/> [support@trackdyne.com](mailto:support@trackdyne.com) | **VigilArc USBL** <br/> Data brief |

<div style="page-break-after: always;"></div>

## Brief description
**VigilArc USBL** is a hydroacoustic ultra-short baseline (USBL) navigation system designed to determine the location of underwater objects marked with hydroacoustic responder beacons [VigilArc Tag](VigilArc_Tag_Specification_en.md) using a direction-finding transceiver antenna [VigilArc Array](VigilArc_Array_Specification_en.md).

<div style="page-break-after: always;"></div>

## System Composition

|  |  |
| :---: | :--- |
| ![VigilArc Array](/documentation/vigilarc_array.png) | [VigilArc Array](VigilArc_Array_Specification_en.md) <br/> Direction-finding antenna |
| ![VigilArc Tag](/documentation/vigilarc_tag_wbat.png) | [VigilArc Tag](VigilArc_Tag_Specification_en.md) <br/> Responder-beacons (one base station can work with a maximum of 16 transponders in sequence) |
|  | [VigilArc Deck](VigilArc_Deck_Specification_en.md) <br/> Autonomous power supply |

<div style="page-break-after: always;"></div>

## Tasks to be solved by the system
* Determining the location of up to 16 underwater objects in water area (tracking underwater objects)
* Relative location determination (**azimuth, distance, depth**)
* Absolute positioning (**latitude, longitude, azimuth, distance, depth**) when connected to an external **GNSS** and compass (or **GNSS with compass function**)

<div style="page-break-after: always;"></div>

## Distinctive features
* Compactness, long range and maximum ease of use make it possible to use the **VigilArc** system to work with various **ROV** and **AUV**, as well as with **divers** in any combination
* High versatility of responders allows them to be used as a stand-alone version with a separate battery pack, as well as energetically and informationally connected with a vessel
* The system supports integration with external sources of navigation data: **GNSS** with compass function (connected to the control PC). In this case, the system determines the absolute geographical coordinates of underwater objects, allows you to save a track of movement of underwater objects and has GPS emulation functions for one of the selected beacons for integration with third-party software (for example, Hypack, SAS.Planet, etc.)
* Antenna VigilArc Array is installed on a boom from almost any vessel, connected to a 12 V / 3.5 A power source, and to a control PC (Windows 10 and higher) - in this minimum configuration, the system determines the position of the responders (azimuth and distance) relative to the antenna. When a GNSS receiver with a compass function (**RMC, GGA, HDG**) is connected to the control PC, the system determines the geographic coordinates of the responders and can transmit them (**RMC, GGA**) to any serial port, thereby emulating a GNSS receiver for the selected responder beacon;
<div style="page-break-after: always;"></div>

<table>
<thead><tr><th align="center" markdown="span">![VigilArc Array placement](/documentation/vigilarc_boat_gnss_1.png)</th></tr></thead>
<tbody>
<tr><td align="center" markdown="span">[VigilArc Array](VigilArc_Array_Specification_en.md) deployment scheme <br/> _The antenna is mounted on a rigid rod so that it is no closer than 2 meters from the surface of the water and no closer than 1.5 meters from the bottom of the vessel. The antenna offsets relative to the geolocation point and the angular offset of the zero of the antenna and the GNSS compass are set_</td></tr>
</tbody>
</table>

<div style="page-break-after: always;"></div>

## Pairing schemes

### Work in relative coordinates
To determine the **relative location** of the responder beacons, the antenna is interfaced with a PC on which specialized host software AzimuthSuite (available on request from [support@trackdyne.com](mailto:support@trackdyne.com)) is installed. The antenna is connected to the PC via [VigilArc Deck](VigilArc_Deck_Specification_en.md), which converts the interface to USB and powers the antenna.

In this case, the following data and functions are available to the user:
* **Azimuth** (horizontal angle) to the used transponder beacons;
* **Distance** to responder beacons
* **Depths** of transponder beacons

<table>
<thead><tr><th align="center" markdown="span">![VigilArc Array relative scheme](/documentation/vigilarc_option1.png)</th></tr></thead>
<tbody>
<tr><td align="center" markdown="span">_Working in relative coordinates_</td></tr>
</tbody>
</table>

<div style="page-break-after: always;"></div>

### Working in absolute coordinates
To determine the **absolute location** of the responder beacons, the antenna is interfaced with a PC on which specialized control software AzimuthSuite (available on request from [support@trackdyne.com](mailto:support@trackdyne.com)) is installed. The antenna is connected to the PC via [VigilArc Deck](VigilArc_Deck_Specification_en.md), which converts the interface to USB and powers the antenna. Additionally, an external **GNSS** system with compass function operating under the **NMEA 0183** protocol (**RMC** and **HDT** messages) is connected.

<table>
<thead><tr><th align="center" markdown="span">![VigilArc Array absolute scheme](/documentation/vigilarc_option2.png)</th></tr></thead>
<tbody>
<tr><td align="center" markdown="span">_Working in absolute coordinates_</td></tr>
</tbody>
</table>

In this case, the following data and functions are available to the user:
* Absolute **geographical coordinates** of responders and their depths
* **Azimuth** (relative to North)
* **Distance**
* Recording a track of the movement of underwater objects with the possibility of subsequent saving in Google KML format.

<div style="page-break-after: always;"></div>

## Geometric Constraints

Since the location of [VigilArc Tag](VigilArc_Tag_Specification_en.md) responder beacons is carried out by the horizontal angle of arrival of the signal, slant range and depth difference, the [VigilArc Array](VigilArc_Array_Specification_en.md) direction finding station antenna array has the highest sensitivity in the range angles from 0° to 85° from the horizontal. The accuracy of the system when the responder is close to the nadir direction may be reduced.

<table>
<thead><tr><th align="center" markdown="span">![VigilArc Array angular zones](/documentation/vigilarc_geometric_limitations.png)</th></tr></thead>
<tbody>
<tr><td align="center" markdown="span">Geometric constraints [VigilArc Array](VigilArc_Array_Specification_en.md) <br/> _1 - DF antenna, 2 - upper hemisphere, 3 - working area (0° .. 85°, 0 .. -85°), 4 - area of accuracy reduction (85° .. -85°)_</td></tr>
</tbody>
</table>

<div style="page-break-after: always;"></div>

_________  

<table>
<thead><tr><th align="left" markdown="span">**Additional information**</th></tr></thead>
<tbody>
<tr><td align="left" markdown="span">[**VigilArc USBL**: User's manual](VigilArc_Users_manual_en.md)</td></tr>
<tr><td align="left" markdown="span">[**VigilArc Tag**: Responder beacon, device specification](VigilArc_Tag_Specification_en.md)</td></tr>
<tr><td align="left" markdown="span">[**VigilArc Array**: DF-antenna, device specification](VigilArc_Array_Specification_en.md)</td></tr>
<tr><td align="left" markdown="span">[**VigilArc Deck**: Autonomous power supply, device specification](VigilArc_Deck_Specification_en.md)</td></tr>
<tr><td align="left" markdown="span">[**VigilArc USBL: Communication protocol specification**](VigilArc_Protocol_Specification_en.md)</td></tr>
</tbody>
</table>
