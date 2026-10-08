[Main](/) ❯ [Navigation & tracking systems](/navigation_and_tracking_systems_en) ❯ **AsterGrid: Databrief**

<div style="page-break-after: always;"></div>

| ![logo](/documentation/logo.svg) |  |
| :---: | ---: |
| [trackdyne.com](https://trackdyne.com/) <br/> [support@trackdyne.com](mailto:support@trackdyne.com) | **AsterGrid**<br/> Data brief |

<div style="page-break-after: always;"></div>

## General information
**AsterGrid** is a system that implements the so-called "underwater GPS", following the ideology of satellite 
navigation systems as closely as possible, it allows an unlimited number of underwater objects, such as divers and various mobile robots (ROV, AUV, etc.) to determine
its geographical location and depth in real-time.

**AsterGrid** is a long-base (LBL, long-baseline) navigation system. The floating navigation base is formed by four small-sized
sonobuoys [AsterGrid Buoy](AsterGrid_Buoy_Specification_en.md); an unlimited number of underwater objects equipped with navigation receivers [AsterGrid Node](AsterGrid_Node_Specification_en.md) and divers using diving navigators [AsterGrid Nav](AsterGrid_Nav_Specification_en.md) can work simultaneously with the support of the base.



<div style="page-break-after: always;"></div>

## System composition

|  |  |
| :---: | :--- |
|  | [AsterGrid Buoy](AsterGrid_Buoy_Specification_en.md) <br/> GNSS-equipped sonobuoy |
| ![AsterGrid Node](/documentation/def_modem_black.png) | [AsterGrid Node](AsterGrid_Node_Specification_en.md) <br/> Navigation receiver |
|  | [AsterGrid Nav](AsterGrid_Nav_Specification_en.md) <br/> Diver's navigation received |

The minimum composition of the system includes four sonobuoys [AsterGrid Buoy](AsterGrid_Buoy_Specification_en.md) and one receiving device, 
depending on the user task:
* If you want to provide navigation data to the diver, then use the diving navigator [AsterGrid Nav](AsterGrid_Nav_Specification_en.md);
* If it is required to estimate the location of the remote-controlled device (ROV, AUV), then the navigation receiver 
[AsterGrid Node](AsterGrid_Node_Specification_en.md) is used, which is interfaced with the vessel, and the data generated at the receiver must be 
transmitted via the cable of the device to the control panel, where they can be displayed on any mapping software that supports the 
connection of standard GNSS receivers (RMC and GGA messages).

<div style="page-break-after: always;"></div>

## Tasks that the system solves
* Simultaneous estimation of 3D geographical position by an unlimited number of underwater objects (divers, ROV, AUV, etc.);
* Recording tracks of divers moving;
* Pre-loading waypoints, navigation to loaded points, saving (marking) the current position of the diver;

<div style="page-break-after: always;"></div>

## Distinctive features
* Work in absolute geographical coordinates;
* A floating base of four sonobuoys is enough for an unlimited number of navigation receivers;
* No preliminary adjustment and calibration of the system and its components is required;
* Small size and power consumption of navigation receivers;
* Emulation of the protocol of standard GNSS receivers for integrated devices

<div style="page-break-after: always;"></div>

## Geometric restrictions
In view of the fact that **AsterGrid** system uses modern technology of digital broadband acoustic communication, the signals emitted by 
buoys have a significant duration (about 200 milliseconds). The buoy's signals have time and code division multiplexing, and in view of 
the finiteness of the speed of sound propagation in water and the period of emission of signals, under certain conditions, the signals 
can overlap each other at the receiving point. There are also limitations associated with the physical basis of the long navigation base.
Therefore, the system has a restriction on the relative position of navigation sonobuoys, and navigation receivers relative to buoys:
* _From each to each of the buoys there should be no more than 700 meters and not less than 30 meters_
* _Buoys should be located with a convex quadrangle so that its sides are approximately equal and differ by no more than 2 times_
* _Maximum immersion depth of navigation receivers should not exceed the size of the navigation base_
* _The highest accuracy of the system is achieved inside the figure of buoys, and work should always begin inside this figure. 
Going beyond the limits of the figure is possible, however, the accuracy can significantly decrease as the positioned object moves away 
from the figure of buoys_

<div style="page-break-after: always;"></div>

_________  

| **Additional information** |
| :--- |
| [Tracks](media.md) |
| [AsterGrid Buoy - GNSS-equipped sonobuoy: Device specification](AsterGrid_Buoy_Specification_en.md) |
| [AsterGrid Nav - Diver's navigation receiver: Device specification](AsterGrid_Nav_Specification_en.md) |
| [AsterGrid Node - navigation receiver: Device specification](AsterGrid_Node_Specification_en.md) |
| [AsterGrid - AsterGrid Node interfacing protocol description](AsterGrid_Protocol_Specification_en.md) |
| [AsterGrid - User's manual](AsterGrid_Users_Manual_en.md) |
