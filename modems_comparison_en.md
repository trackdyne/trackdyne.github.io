[Main](/) ❯ [Underwater acoustic modems](/underwater_acoustic_modems_en.html) ❯ **Modems comparison table**

<div style="page-break-after: always;"></div>

| ![Trackdyne](/documentation/logo.svg) | ![image](/documentation/modems_comparison_en_qr.png) |
| :---: | ---: |
| [trackdyne.com](https://trackdyne.com/) <br/> [support@trackdyne.com](mailto:support@trackdyne.com) | Modems comparison table |

<div style="page-break-after: always;"></div>

## Modems comparison table

|  | [Vexa Mini](/documentation/EN/Vexa/Vexa_Mini_Specification_en.html) | [Vexa Max OEM](/documentation/EN/Vexa/Vexa_Max_OEM_Specification_en.html) | [Vexa Max](/documentation/EN/Vexa/Vexa_Max_Specification_en.html) | [Vexa Locator Modem](/documentation/EN/Vexa/Vexa_Locator_Modem_Specification_en.html) |
| :--- | :---: | :---: | :---: | :---: |
|      |  |  | ![](/documentation/def_modem_black.png) | ![](/documentation/vigilarc_array.png) |
| Current status | **Available** | **Available** | **Available** | **Available** |
| Maximum communication range, m | 1000<sup>[1](#footnote1)</sup> | 3000<sup>[1](#footnote1),[2](#footnote2)</sup> | 3000<sup>[1](#footnote1),[2](#footnote2)</sup> | 3000<sup>[1](#footnote1),[2](#footnote2)</sup> |
| Data rate, bit/s | 78 / 156<sup>[3](#footnote3)</sup> / 314<sup>[3](#footnote3)</sup> / 634<sup>[3](#footnote3)</sup> | 78 / 156<sup>[3](#footnote3)</sup> / 314<sup>[3](#footnote3)</sup> / 634<sup>[3](#footnote3)</sup> | 78 / 156<sup>[3](#footnote3)</sup> / 314<sup>[3](#footnote3)</sup> / 634<sup>[3](#footnote3)</sup> | 78 / 156<sup>[3](#footnote3)</sup> / 314<sup>[3](#footnote3)</sup> / 634<sup>[3](#footnote3)</sup> |
| Dimensions, mm | **Ø41 x 45** | 80 x 43 x 29 (PCB) <br/> Ø64 x 62 (transducer) |  Ø64 x 62 | Ø64 x 128 |
| Weight (dry), g | **160** | 54 (PCB) <br/> 360 (transducer) | 360 | 440 |
| Maximum operating depth, m | 300 | **400 / 1000** <sup>[4](#footnote4),[5](#footnote5)</sup> | 300 | 300 |
| Supply voltage<sup>[6](#footnote6)</sup>, V | 5 .. 12 | 5 .. 12 | 5 .. 12 | 5 .. 12 |
| Power consumption (RX/TX), W | **0.33/6** | 0.33/15 | 0.33/15 | 0.33/15 |
| Maximum acoustic source level (in band), dB re 1 μPa @ 1 m | 169 | 175 | 175 | 175 |
| Connection interface | UART | UART | UART | UART |
| Code division multiple access | **✓** | **✓** | **✓** | **✓** |
| Logical addressing | **✓** | **✓** | **✓** | **✓** |
| Packet mode with guaranteed delivery | **✓** | **✓** | **✓** | **✓** |
| Propagation time measurement function | **✓** | **✓** | **✓** | **✓** |
| Supply voltage measurement module | **✓** | **✓** | **✓** | **✘** |
| Depth/temperature sensor | **✓** | **✘** | **✓** | **✓** |
| Two-axis inclinometer | **✘** | **✘** | **✘** | **✓** |
| Determination of the horizontal angle of arrival of the signal | **✘** | **✘** | **✘** | **✓** |

________________

<a name="footnote1"><sup>1</sup></a> A parameter that determines the maximum range at which a signal can be received based on the electroacoustic parameters of the transmitter and receiver, spatial decrease in the intensity of sound energy, attenuation in the medium and underwater acoustic noise level.  
<a name="footnote2"><sup>2</sup></a> When [Vexa Max OEM](/documentation/EN/Vexa/Vexa_Max_OEM_Specification_en.html), [Vexa Max](/documentation/EN/Vexa/Vexa_Max_Specification_en.html) and [Vexa Locator Modem](/documentation/EN/Vexa/Vexa_Locator_Modem_Specification_en.html) operate in any combination. The maximum communication range with standard [Vexa Mini](/documentation/EN/Vexa/Vexa_Mini_Specification_en.html) modems is 1000 meters. The parameter is specified for the standard data rate mode - 78 bit/s.  
<a name="footnote3"><sup>3</sup></a> The standard data rate mode of 78 bit/s provides maximum communication range and noise immunity. Other modes are available by reflashing the devices.  
<a name="footnote4"><sup>4</sup></a> The maximum depth is determined by the transducer. The modem's printed circuit board must be located in the user's one-atmosphere (normobaric) housing.  
<a name="footnote5"><sup>5</sup></a> An operating depth of 1000 meters is achieved when using the deep-water transducer.  
<a name="footnote6"><sup>6</sup></a> Maximum power and communication range are achieved at a supply voltage of 12 V.
