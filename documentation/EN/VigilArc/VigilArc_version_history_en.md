[Main](/) ❯ [Navigation & tracking systems](/navigation_and_tracking_systems_en.html) ❯ **VigilArc: Version history & changes**

<div style="page-break-after: always;"></div>

| ![Trackdyne](/documentation/logo.svg) |  |
| :---: | ---: |
| [trackdyne.com](https://trackdyne.com/) <br/> [support@trackdyne.com](mailto:support@trackdyne.com) | **VigilArc** USBL tracking system <br/> Version history & changes |

# VigilArc <br/> Version history & changes

<div style="page-break-after: always;"></div>

## 0. Versions

| Device | Current firmware version | Release date |
| :--- | :--- | :--- |
| VigilArc Array | 2.00 | 10-JAN-2026 |
| VigilArc Tag | 2.00 | 10-JAN-2026 |
| VigilArc Microtag | 2.00 | 10-JAN-2026 |

## 1. Version histories by device

### 1.1. VigilArc Array

| Date | Firmware version | Description |
| :--- | :--- | :--- |
| 10-JAN-2026 | 2.00 | + isolation of uplink channels to increase reliability in challenging conditions. **This version is only partially compatible with previous ones** |
| 26-MAR-2025 | 1.34 | + supply voltage request from the beacon <br/> BUGFIX: error in the automatic speed of sound calculation in the VigilArc Array station |
| 26-DEC-2023 | 1.33 | + telemetry transmission. Up to 28 integer parameters can be assigned to a beacon, which the station can poll. The fact of polling is passed to the control system to implement the remote control function. For more details, see the protocol commands [H2D_CREQ](/documentation/EN/VigilArc/VigilArc_Protocol_Specification_en.html#210-h2d_creq) and [D2D_CSET](/documentation/EN/VigilArc/VigilArc_Protocol_Specification_en.html#211-h2d_cset) |
| 12-APR-2023 | 1.32 | BUGFIX: fixed an error that could cause the station to continue polling the beacons after the connection was closed |
| 10-DEC-2022 | 1.31 | + minor improvements |
| 10-OCT-2022 | 1.30 | |

### 1.2. VigilArc Tag

| Date | Firmware version | Description |
| :--- | :--- | :--- |
| 10-JAN-2026 | 2.00 | + isolation of uplink channels to increase reliability in challenging conditions. **This version is only partially compatible with previous ones** |
| 26-MAR-2025 | 1.34 | + supply voltage transmission on request from the station |
| 26-DEC-2023 | 1.33 | + telemetry transmission. Up to 28 integer parameters can be assigned to a beacon, which the station can poll. The fact of polling is passed to the control system to implement the remote control function. For more details, see the protocol commands [H2D_CREQ](/documentation/EN/VigilArc/VigilArc_Protocol_Specification_en.html#210-h2d_creq) and [D2D_CSET](/documentation/EN/VigilArc/VigilArc_Protocol_Specification_en.html#211-h2d_cset) |
| 01-MAR-2023 | 1.32 | BUGFIX: fixed an error in depth transmission over the underwater acoustic channel |
| 12-FEB-2022 | 1.31 | - minor improvements and refactoring |

________  

<div style="page-break-after: always;"></div>
