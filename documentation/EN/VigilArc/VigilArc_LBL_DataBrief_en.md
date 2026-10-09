[Main](/) ❯ [Navigation & tracking systems](/navigation_and_tracking_systems_en.html) ❯ **VigilArc LBL: Data brief**

<details>
  <summary><b>ℹ Recommendations for printing / saving as PDF</b></summary>
  <br>
  <ol>
    <li>Press <b>Ctrl+P</b> (macOS: <b>Cmd+P</b>)</li>
    <li>Select <b>"Save as PDF"</b> (Microsoft Print to PDF) as the printer</li>
    <li>In <b>"Pages"</b>, enter a range that excludes the first and the last page</li>
    <li>Disable <b>headers and footers</b> (title, URL, page numbers)</li>
    <li>In <b>Chrome/Edge</b>: More settings → "Margins" → <b>None</b> | in <b>Firefox</b>: "Margins & Header/Footer" → <b>None</b></li>
    <li>Click <b>Print</b> and choose where to save the PDF</li>
  </ol>
</details>

<div style="page-break-after: always;"></div>

| ![Trackdyne](/documentation/logo.svg) |  |
| :---: | ---: |
| [trackdyne.com](https://trackdyne.com/) <br/> [support@trackdyne.com](mailto:support@trackdyne.com) | **VigilArc LBL** <br/> Data brief |

<div style="page-break-after: always;"></div>

## General information

**VigilArc LBL** is an underwater acoustic long baseline (LBL) navigation system designed to determine the location of an underwater object using a navigation base formed by [VigilArc Tag](/documentation/EN/VigilArc/VigilArc_Tag_Specification_en.html) responder-beacons.

The system is built on a **single hardware platform**: the [VigilArc L](/documentation/EN/VigilArc/VigilArc_L_Specification_en.html) and [VigilArc LX](/documentation/EN/VigilArc/VigilArc_LX_Specification_en.html) transceivers can be reprogrammed into each other. This makes it possible to change the system configuration to suit the task without replacing the equipment.

<div style="page-break-after: always;"></div>

## System composition

|  |  |
| :---: | :--- |
| ![VigilArc L](/documentation/vigilarc_lbl_transceiver.png) | [VigilArc L](/documentation/EN/VigilArc/VigilArc_L_Specification_en.html) <br/> LBL transceiver with a common request to the navigation base (3–4 responder-beacons with addresses 1-4) |
| ![VigilArc LX](/documentation/vigilarc_lbl_transceiver.png) | [VigilArc LX](/documentation/EN/VigilArc/VigilArc_LX_Specification_en.html) <br/> LBL transceiver with sequential interrogation of up to 4 responder-beacons with arbitrary addresses |
|  | [VigilArc SL](/documentation/EN/VigilArc/VigilArc_SL_Specification_en.html) <br/> Solver: position calculation and GNSS emulation |
| ![VigilArc Tag](/documentation/vigilarc_tag_wbat.png) | [VigilArc Tag](/documentation/EN/VigilArc/VigilArc_Tag_Specification_en.html) <br/> Reference responder-beacons |

<div style="page-break-after: always;"></div>

## System configuration options

The **VigilArc LBL** system can be assembled in one of three modes, depending on the required update rate, the number of responder-beacons and where the result is to be calculated.

### Mode 1. VigilArc L – maximum update rate

The [VigilArc L](/documentation/EN/VigilArc/VigilArc_L_Specification_en.html) transceiver sends a **common (broadcast) request** to a fixed navigation base of **3 or 4 responder-beacons** with fixed addresses 1-4. The responder-beacons reply after fixed delays that depend on their address. The position is calculated by an **external application** on the user's side.

- **Advantages:** maximum position update rate, minimum latency. Possibility of placing the responder-beacons on a moving platform (the bottom of a vessel) with the coordinate system tied to the platform.
- **Limitations:** fixed responder-beacon addresses, the position is calculated by external software, all reference responder-beacons must be within a circle of 265 meters radius.

### Mode 2. VigilArc LX – arbitrary set of responder-beacons

The [VigilArc LX](/documentation/EN/VigilArc/VigilArc_LX_Specification_en.html) transceiver **sequentially interrogates** 3 or 4 responder-beacons with arbitrary addresses and measures the range to each of them. The results are transmitted over UART to an external computing unit – the [VigilArc SL](/documentation/EN/VigilArc/VigilArc_SL_Specification_en.html) module.

- **Advantages:** flexibility – responder-beacons with arbitrary addresses.
- **Limitations:** the update rate is lower than that of VigilArc L, because the interrogation is sequential.

### Mode 3. VigilArc LX + VigilArc SL – standalone position calculation

The [VigilArc LX](/documentation/EN/VigilArc/VigilArc_LX_Specification_en.html) + [VigilArc SL](/documentation/EN/VigilArc/VigilArc_SL_Specification_en.html) combination provides a **ready-made solution**: LX measures the ranges, SL stores the coordinates of the responder-beacons, calculates the position and outputs it to the user in the form of standard **GNSS sentences** (GGA, RMC, MTW). This makes it possible to connect the system wherever a regular GNSS receiver is expected.

- **Advantages:** no external software is needed, the output is a familiar GNSS stream.
- **Limitations:** the update rate is determined by the rate of the sequential interrogation by LX.

<div style="page-break-after: always;"></div>

## Comparison of modes

| Characteristic | VigilArc L | VigilArc LX | VigilArc LX + VigilArc SL |
| :--- | :---: | :---: | :---: |
| Number of responder-beacons | 3–4 | 3–4 | 3–4 |
| Interrogation scheme | common request | sequential | sequential |
| Position calculation | external software | external software | **VigilArc SL** |
| Output | ranges | ranges | **GGA, RMC, MTW** |
| Relative update rate | maximum | medium | medium |

<div style="page-break-after: always;"></div>

## Tasks to be solved

* Determining the location of an object in a local coordinate system (x, y, z) if the positions of the reference responder-beacons are specified in a local Cartesian coordinate system
* Determining the absolute location (**latitude, longitude, depth**) if the positions of the reference responder-beacons are specified in a geographic coordinate system

<div style="page-break-after: always;"></div>

## Distinctive features

* Compactness, long range and maximum ease of use make it possible to use the **VigilArc** system to work with various **ROVs** and **AUVs** as well as with **divers**
* The high versatility of the responder-beacons makes it possible to use them either in a standalone version with a separate battery pack or integrated with the carrier for both power and data
* A **single hardware platform** for the transceivers and the solver: the role of a device is changed by changing the firmware
* A **unique feature** of the system is the possibility of placing the reference points on a moving base, for example, on the bottom of a vessel, so that the positioned object is tied to a coordinate system associated with the moving vessel

<div style="page-break-after: always;"></div>

## Geometric limitations

### VigilArc L mode (common request)
- the reference points must be located within a circle of **265 m** radius, but no closer than **40 m** to each other;
- the limitation is due to the TDMA interrogation scheme: the responder-beacons reply according to their address with a fixed delay;
- continuous line of sight through the water column between the transceiver and all reference points is required for the system to operate.

### VigilArc LX mode (sequential interrogation)
- **there are no restrictions on the geometry of the base** - responder-beacons with arbitrary addresses can be used;
- the positions of the reference responder-beacons are determined in advance, for example, by the VLBL method;
- the only limitation is the **acoustic communication range determined by the link budget, up to 3000 m<sup>[1]</sup>**;
- continuous line of sight through the water column between the transceiver and all reference points is required for the system to operate.
<div style="page-break-after: always;"></div>

_________

<table>
<thead><tr><th align="center" markdown="span">**Additional information**</th></tr></thead>
<tbody>
<tr><td align="center" markdown="span">[Responder-beacon **VigilArc Tag**: device specification](/documentation/EN/VigilArc/VigilArc_Tag_Specification_en.html)</td></tr>
<tr><td align="center" markdown="span">[LBL transceiver **VigilArc L**: device specification](/documentation/EN/VigilArc/VigilArc_L_Specification_en.html)</td></tr>
<tr><td align="center" markdown="span">[LBL transceiver **VigilArc LX**: device specification](/documentation/EN/VigilArc/VigilArc_LX_Specification_en.html)</td></tr>
<tr><td align="center" markdown="span">[Solver **VigilArc SL**: device specification](/documentation/EN/VigilArc/VigilArc_SL_Specification_en.html)</td></tr>
<tr><td align="center" markdown="span">[Communication protocol specification for the devices of the **VigilArc** system](/documentation/EN/VigilArc/VigilArc_Protocol_Specification_en.html)</td></tr>
</tbody>
</table>
