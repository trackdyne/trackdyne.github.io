[Main](/) ❯ [Underwater acoustic modems](/underwater_acoustic_modems_en) ❯ **Modems comparison table**

<div style="page-break-after: always;"></div>

| ![Trackdyne](/documentation/logo.png) |  |
| :---: | ---: |
| [trackdyne.com](https://trackdyne.com/) <br/> [support@trackdyne.com](mailto:support@trackdyne.com) | Modems comparison table |

<div style="page-break-after: always;"></div>

## Modems comparison table

|  | [Vexa Mini](/documentation/EN/Vexa/Vexa_Mini_Specification_en.md) | [Vexa Max OEM](/documentation/EN/Vexa/Vexa_Max_OEM_Specification_en.md) | [Vexa Max](/documentation/EN/Vexa/Vexa_Max_Specification_en.md) | [Vexa Locator Modem](/documentation/EN/Vexa/Vexa_Locator_Modem_Specification_en.md) |
| :--- | :---: | :---: | :---: | :---: |
|      | ![](/documentation/vexa_mini_transducer.png) |  | ![](/documentation/def_modem_black.png) | ![](/documentation/vigilarc_array.png) |
| Status | **Active** | **Active** | **Active** | **Active** |
| Max. acoustic range, m | 1000<sup>[1](#footnote1)</sup> | 3000<sup>[1](#footnote1),[2](#footnote2)</sup> | 3000<sup>[1](#footnote1),[2](#footnote2)</sup> | 3000<sup>[1](#footnote1),[2](#footnote2)</sup> |
| Baudrate, bps | 78 / 156<sup>[3](#footnote3)</sup> / 314<sup>[3](#footnote3)</sup> / 634<sup>[3](#footnote3)</sup> | 78 / 156<sup>[3](#footnote3)</sup> / 314<sup>[3](#footnote3)</sup> / 634<sup>[3](#footnote3)</sup> | 78 / 156<sup>[3](#footnote3)</sup> / 314<sup>[3](#footnote3)</sup> / 634<sup>[3](#footnote3)</sup> | 78 / 156<sup>[3](#footnote3)</sup> / 314<sup>[3](#footnote3)</sup> / 634<sup>[3](#footnote3)</sup> |
| Dimensions, mm | **Ø41 x 45** | 80 x 43 x 29 (PCB) <br/> Ø64 x 62 (transducer) |  Ø64 x 62 | Ø64 x 128 |
| Weight (dry), g | **160** | 54 (PCB) <br/> 360 (transducer) | 360 | 440 |
| Depth rating, m | 300 | **400 / 1000** <sup>[4](#footnote4),[5](#footnote5)</sup> | 300 | 300 |
| Supply voltage<sup>[6](#footnote6)</sup>, V | 5 .. 12 | 5 .. 12 | 5 .. 12 | 5 .. 12 |
| Power consumption (RX/TX), W | **0.33/6** | 0.33/15 | 0.33/15 | 0.33/15 |
| Acoustic source level (in band), dB re 1 uPa @ 1 m | 169 | 175 | 175 | 175 |
| Interface | UART | UART | UART | UART |
| Supscribers code division | **✓** | **✓** | **✓** | **✓** |
| Logical addressing | **✓** | **✓** | **✓** | **✓** |
| Packet mode with guaranteed delivery | **✓** | **✓** | **✓** | **✓** |
| Propagation time measurement | **✓** | **✓** | **✓** | **✓** |
| Supply voltage measurement circuit | **✓** | **✓** | **✓** | **✘** |
| Depth/Temperature sensor | **✓** | **✘** | **✓** | **✓** |
| Dual axis inclinometer | **✘** | **✘** | **✘** | **✓** |
| Determining the horizontal angle of arrival | **✘** | **✘** | **✘** | **✓** |

________________

<a name="footnote1"><sup>1</sup></a> A parameter that determines the maximum range at which a signal can be received based on the electro-acoustic parameters of the transmitter and receiver, spatial decrease in the intensity of sound energy, attenuation in the medium and acoustic noise level.  
<a name="footnote2"><sup>2</sup></a> When communicating [Vexa Max OEM](/documentation/EN/Vexa/Vexa_Max_OEM_Specification_en.md), [Vexa Max](/documentation/EN/Vexa/Vexa_Max_Specification_en.md) and [Vexa Locator Modem](/documentation/EN/Vexa/Vexa_Locator_Modem_Specification_en.md) in any combination. The maximum communication range with standard modems [Vexa Mini](/documentation/EN/Vexa/Vexa_Mini_Specification_en.md) is 1000 meters. The parameter is specified for the standard speed mode - 78 bps.  
<a name="footnote3"><sup>3</sup></a> Standard speed mode 78 bps provides maximum communication range and noise immunity. Other modes are available by [re-flashing devices](/documentation/EN/Vexa/Vexa_FW_Updating_en.md).  
<a name="footnote4"><sup>4</sup></a> The maximum depth is determined by the transducer. The modem's printed circuit board must be located in the user's normobaric enclosure.  
<a name="footnote5"><sup>5</sup></a> Working depth of 1000 meters is ensured when working with the deep-water transducer option.   
<a name="footnote6"><sup>6</sup></a> Maximum power and communication range is provided at a supply voltage of 12 V.

<div style="page-break-after: always;"></div>
