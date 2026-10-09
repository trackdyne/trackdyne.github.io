[Main](/) ❯ [Navigation & tracking systems](/navigation_and_tracking_systems_en.html) ❯ **Comparison table of navigation systems**

<div style="page-break-after: always;"></div>

| ![Trackdyne](/documentation/logo.svg) | ![image](/documentation/navigation_systems_comparison_en_qr.png) |
| :---: | ---: |
| [trackdyne.com](https://trackdyne.com/) <br/> [support@trackdyne.com](mailto:support@trackdyne.com) | Comparison of navigation and tracking systems |

<div style="page-break-after: always;"></div>

## Comparison table of navigation systems

|  | [AsterGrid underwater GPS](/documentation/EN/AsterGrid/AsterGrid_DataBrief_en.html) | [EchoTrace](/documentation/EN/EchoTrace/EchoTrace_DataBrief_en.html) | [EchoTrace](/documentation/EN/EchoTrace/EchoTrace_DataBrief_en.html) + <br/> [SubVox Diver](/documentation/EN/SubVox/SubVox_Diver_Specification_en.html) | [VigilArc USBL](/documentation/EN/VigilArc/VigilArc_DataBrief_en.html) | [Vexa Locator](/documentation/EN/Vexa/Vexa_Locator_Modem_Specification_en.html) |
| :--- | :---: | :---: | :---: | :---: | :---: |
| System type | LBL | LBL | LBL | USBL | USBL |
| Location where navigation information is generated | Underwater <br/> object | Surface <br/> control point | Surface <br/> control point | Surface <br/> control point | Surface <br/> control point |
| Number of positioned objects | **∞** | 1 | up to 255<sup>[1](#footnote1)</sup> | up to 16<sup>[1](#footnote1)</sup> | up to 20<sup>[1](#footnote1)</sup> |
| Nominal navigation data update period | 1 s | 2 s | Position update at the end of each voice message from a diver | ≥ 1<sup>[2](#footnote2)</sup> s | ≥ 3.6<sup>[2](#footnote2)</sup> s |
| Maximum working area size | 700 x 700 m | 1500 x 1500 m | 1500 x 1500 m | circle R = 3000 m | circle R = 1000 m |
| Nominal accuracy | 2DRMS 0.84 m | 2DRMS 0.84 m | 2DRMS 1.5 m | 1° (≈17 m at a distance of 1000 m) | 2° (≈35 m at a distance of 1000 m) |
| Maximum depth | 300<sup>[3](#footnote3)</sup> m | 300/500<sup>[3](#footnote3)</sup><sup>,[4](#footnote4)</sup> m | 100 m | 300/350<sup>[4](#footnote4)</sup> m | 300 m |
| Navigation data generated | Latitude, <br/> Longitude, <br/> Depth, <br/> Temperature, <br/> UTC time<sup>[7](#footnote7)</sup>, <br/> Course | Latitude, <br/> Longitude, <br/> Depth<sup>[5](#footnote5)</sup>, <br/> Temperature<sup>[5](#footnote5)</sup>, <br/> Course | Latitude, <br/> Longitude | Range, <br/> Azimuth, <br/> Depth, <br/> Battery charge, <br/> Latitude<sup>[6](#footnote6)</sup>, <br/> Longitude<sup>[6](#footnote6)</sup> | Range, <br/> Azimuth, <br/> Depth, <br/> Battery charge, <br/> Latitude<sup>[6](#footnote6)</sup>, <br/> Longitude<sup>[6](#footnote6)</sup> |
| Maximum relative velocity | ±1.8 m/s | ±1.8 m/s | ±1.8 m/s | ±2 m/s | ±1 m/s |
| Deployment features | Requires 4 floating buoys to be deployed | Requires 4 floating buoys to be deployed | Requires 4 floating buoys to be deployed | Requires mounting the base station on a rigid pole and connecting an external GPS and compass | Requires mounting the base station on a rigid pole and connecting an external GPS and compass |
| Distinctive feature | - Unlimited number of simultaneously positioned devices.<br/> - No calibration required. <br/> - Ability to connect to the [Aquatab S](https://duslate.com/products/aquatab-s/) diver's tablet | - The fastest and easiest system deployment. <br/> - Diver positioning simultaneously with voice transmission. <br/> - No calibration required. | - The fastest and easiest system deployment. <br/> - Diver positioning simultaneously with voice transmission. <br/> - No calibration required. | - Automatic operation. <br/> - Ability to transmit user telemetry data from the beacon<sup>[8](#footnote8)</sup> | Two-way data transmission |

<div style="page-break-after: always;"></div>
________________  

<a name="footnote1"><sup>1</sup></a> The maximum supported number of responder-beacons is specified; the system works with them sequentially.  
<a name="footnote2"><sup>2</sup></a> The minimum value is indicated when working with one responder-beacon located at a distance of up to 100 meters from the base station.  
<a name="footnote3"><sup>3</sup></a> For the diver version, the maximum depth is 70 m.  
<a name="footnote4"><sup>4</sup></a> Different maximum depths for different system versions.  
<a name="footnote5"><sup>5</sup></a> The parameters are available only when working with the [EchoTrace pinger](/documentation/EN/EchoTrace/EchoTrace_Pinger_Specification_en.html). When positioning diver telephone devices, these parameters are not available.  
<a name="footnote6"><sup>6</sup></a> These parameters are available only when external sources of navigation data are connected: the heading and geographic position of the base station.  
<a name="footnote7"><sup>7</sup></a> These parameters are not available in the diver version of the receiver.  
<a name="footnote8"><sup>8</sup></a> When the responder-beacon is data-interfaced with the carrier, up to 28 different user integer parameters in the range from 0 to 499 can be set. Each of these parameters can be transmitted by the beacon on request from the direction-finding station.  

<div style="page-break-after: always;"></div>
