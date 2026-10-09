[Main](/) ❯ [Navigation & tracking systems](/navigation_and_tracking_systems_en.html) ❯ **AsterGrid Node: Device specification**

<div style="page-break-after: always;"></div>

| ![Trackdyne](/documentation/logo.svg) | ![logo](/documentation/def_modem_black.png) |
| :---: | ---: |
| [trackdyne.com](https://trackdyne.com/) <br/> [support@trackdyne.com](mailto:support@trackdyne.com) | **AsterGrid Node** - Universal navigation receiver <br/> Device specification |

## KEY FEATURES

* **3D position in absolute geographical coordinates**
* **Emulation of the protocol of conventional GNSS receivers**
* **Update rate of 3D position up to 1 Hz**
* **Completely acoustically passive device**
* **Minimum dimensions and weight**
* **Simultaneous operation of an unlimited number of devices**
* **Reliable and noise-resistant digital broadband underwater acoustic communication technology**
* **Monoblock design**

## DESCRIPTION

With the support of four floating navigation sonobuoys [AsterGrid Buoy](/documentation/EN/AsterGrid/AsterGrid_Buoy_Specification_en.html), simultaneous operation of an unlimited number of **AsterGrid Node** and [AsterGrid Nav](/documentation/EN/AsterGrid/AsterGrid_Nav_Specification_en.html) devices is possible in one operating area.  

**AsterGrid Node** is the universal navigation receiver of the **[AsterGrid](/documentation/EN/AsterGrid/AsterGrid_DataBrief_en.html)** system. It receives underwater acoustic navigation signals from the buoys and determines its own geographical coordinates, which it transmits via a serial interface (**UART**) to the control system. It emulates the sentence format used in conventional GNSS receivers, which ensures maximum simplicity of integration.

_________

<div style="page-break-after: always;"></div>

## TECHNICAL SPECIFICATIONS

| PARAMETER | VALUE |
| :--- | :--- |
| DIMENSIONS (REMOTE UNIT, Ø x h) | 64 x 62 mm |
| WEIGHT (dry) | 0.3 kg |
| SUPPLY VOLTAGE<sup>[1](#footnote1)</sup> | 12 V |
| DATA LINE VOLTAGE | 3.3 V |
| DATA LINE OUTPUT IMPEDANCE | 1 kΩ |
| POWER CONSUMPTION | 0.35 W |
| MAXIMUM VELOCITY RELATIVE TO BUOYS | +/- 1.8 m/s |
| OPERATING TEMPERATURE RANGE | -5 .. 50 °C |
| MAXIMUM IMMERSION DEPTH | 300 m |
| MAXIMUM WORKING AREA SIZE | 700 x 700 m inside the buoy figure |
| MAXIMUM ACOUSTIC COMMUNICATION RANGE<sup>[2](#footnote2)</sup> | 3000 m |
| CARRIER FREQUENCY | 20100 Hz |
| MINIMUM SIGNAL-TO-NOISE RATIO (IN BAND)<sup>[3](#footnote3)</sup> | -6 dB |
| REFERENCE ELLIPSOID | WGS-84 |
| NOMINAL HORIZONTAL ACCURACY<sup>[4](#footnote4)</sup> (2DRMS) | 0.84 m |
| NOMINAL DEPTH ACCURACY<sup>[5](#footnote5)</sup> | 0.1 m |
| NOMINAL TIME TO FIRST FIX | 28 s |
| NOMINAL POSITION UPDATE RATE | 1 Hz |
| NOMINAL STARTUP TIME | 100 ms |
| BUILT-IN TEMPERATURE SENSOR ACCURACY | 0.1 °C |
| CABLE LENGTH | 1 m |
| CABLE DIAMETER | 5 mm |
| INTERFACE<sup>[6](#footnote6)</sup> | UART, 9600 |
| COMMUNICATION [PROTOCOL](/documentation/EN/AsterGrid/AsterGrid_Protocol_Specification_en.html) | NMEA0183 (RMC, GGA, WTW) <br/> + extended set of sentences |

________________
<a name="footnote1"><sup>1</sup></a> For devices manufactured after June 2020. For devices manufactured earlier, the supply voltage is 5 V.  
<a name="footnote2"><sup>2</sup></a> A parameter that determines the maximum range at which signal reception is possible, based on the electro-acoustic parameters of the transmitter and receiver, the spatial decrease in the intensity of sound energy, attenuation in the medium and the acoustic noise level.  
<a name="footnote3"><sup>3</sup></a> The value was obtained without taking the multipath propagation effect into account.  
<a name="footnote4"><sup>4</sup></a> The value was obtained by measurement in a real body of water with the buoys and the navigation receiver fixed in place for 60 minutes.  
<a name="footnote5"><sup>5</sup></a> The value may depend on the correctness of the salinity of the water in which the work is performed, as set by the user.  
<a name="footnote6"><sup>6</sup></a> By agreement, the device can be supplied with an RS422 interface converter mounted on the cable in a maintenance-free urethane housing.  

<div style="page-break-after: always;"></div>
