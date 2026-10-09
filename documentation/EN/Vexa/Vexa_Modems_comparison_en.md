[Main](/) ❯ [Underwater acoustic modems](/underwater_acoustic_modems_en) ❯ **Vexa family modems comparison tables**

<div style="page-break-after: always;"></div>

| ![Trackdyne](/documentation/logo.svg) | |
| :---: | ---: |
| [trackdyne.com](https://trackdyne.com/) <br/> [support@trackdyne.com](mailto:support@trackdyne.com) | **Vexa Mini** modems comparison |

<div style="page-break-after: always;"></div>

## Main features

|  | [Vexa Mini](Vexa_Mini_Specification_en.md) | [Vexa Max OEM](Vexa_Max_OEM_Specification_en.md) | [Vexa Max](Vexa_Max_Specification_en.md) | [Vexa Locator Modem](Vexa_Locator_Modem_Specification_en.md) | 
| :--- | :---: | :---: | :---: | :---: | 
|      | ![](/documentation/vexa_mini_transducer.png) |  | ![](/documentation/def_modem_black.png) | ![](/documentation/def_vigilarc_array_ant.png) |
| Status | **Active** | **Active** | **Active** | **Active** |
| Max. acoustic range, m | 1000<sup>[1](#footnote1)</sup> | 3000<sup>[1](#footnote1),[2](#footnote2)</sup> | 3000<sup>[1](#footnote1),[2](#footnote2)</sup> | 3000<sup>[1](#footnote1),[2](#footnote2)</sup> |
| Baudrate, bps | 78 / 156<sup>[3](#footnote3)</sup> / 314<sup>[3](#footnote3)</sup> / 634<sup>[3](#footnote3)</sup> | 78 / 156<sup>[3](#footnote3)</sup> / 314<sup>[3](#footnote3)</sup> / 634<sup>[3](#footnote3)</sup> | 78 / 156<sup>[3](#footnote3)</sup> / 314<sup>[3](#footnote3)</sup> / 634<sup>[3](#footnote3)</sup> |78 / 156<sup>[3](#footnote3)</sup> / 314<sup>[3](#footnote3)</sup> / 634<sup>[3](#footnote3)</sup> |
| Dimensions, mm | **Ø41 x 45** | 80 x 43 x 29 (PCB) <br/> Ø64 x 62 (transducer) | Ø64 x 62 | Ø64 x 128 |
| Weight (dry), g | **160** | (PCB) 54 <br/> (transducer) 360 | 360 | 440 |
| Depth rating, m | 300 | **400 / 1000** <sup>[4](#footnote4),[5](#footnote5)</sup> | 300 | 300 |
| Power consumption (RX/TX), W | 0.33/6 | 0.33/15 | 0.33/15 | 0.33/15 |
| Acoustic source level (in band), dB re 1 uPa @ 1 m | 169 | 175 | 175 | 175 |
| Supply voltage measurement | **✓** | **✓** | **✓** | **✘** |
| Depth/temperature sensor | **✓** | **✘** | **✓** | **✓** |
| 2-Axis inclinometer | **✘** | **✘** | **✘** | **✓** |
| Horizontal angle of arrival estimation | **✘** | **✘** | **✘** | **✓** |

## Data transmission speed options

All devices of the family can work with alternative firmware supporting different communication speed modes.
The modes are not compatible with each other. Mode change is made by [flashing the device](Vexa_FW_Updating_en.md).

|      | STRONG | EASY   | LITE   | HASTE |
| :--- | :---:  | :---:  | :---:  | :---:  |
| Baudrate, bps | 78 | 156 | 314 | 634 |
| Max. acoustic range, m | 1000/3000<sup>[1](#footnote1),[2](#footnote2)</sup> | 800<sup>[1](#footnote1)</sup> | 700<sup>[1](#footnote1)</sup> | 500<sup>[1](#footnote1)</sup> |
| Number of code channels | 20 | 14 | 7 | 3 |


<div style="page-break-after: always;"></div>

________________
<a name="footnote1"><sup>1</sup></a> A parameter that determines the maximum range at which a signal can be received based on the electro-acoustic parameters of the transmitter and receiver, spatial decrease in the intensity of sound energy, attenuation in the medium and acoustic noise level.  
<a name="footnote2"><sup>2</sup></a> When communicating [Vexa Max OEM](Vexa_Max_OEM_Specification_en.md), [Vexa Max](Vexa_Max_Specification_en.md) and [Vexa Locator Modem](Vexa_Locator_Modem_Specification_en.md) in any combination. The maximum communication range with standard modems [Vexa Mini](Vexa_Mini_Specification_en.md) is 1000 meters. The parameter is specified for the standard speed mode - 78 bps.  
<a name="footnote3"><sup>3</sup></a> Standard speed mode 78 bps provides maximum communication range and noise immunity. Other modes are available by [re-flashing devices](Vexa_FW_Updating_en.md).  
<a name="footnote4"><sup>4</sup></a> The maximum depth is determined by the transducer. The modem's printed circuit board must be located in the user's normobaric enclosure.  
<a name="footnote5"><sup>5</sup></a> Working depth of 1000 meters is ensured when working with the deep-water transducer option.   

  
<div style="page-break-after: always;"></div>
