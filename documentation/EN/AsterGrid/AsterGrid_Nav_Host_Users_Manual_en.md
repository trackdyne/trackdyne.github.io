[Main](/) ❯ [Navigation & tracking systems](/navigation_and_tracking_systems_en.html) ❯ **AsterGrid Nav Host: User's manual**

<div style="page-break-after: always;"></div>

| ![Trackdyne](/documentation/logo.svg) |  |
| :---: | ---: |
| [trackdyne.com](https://trackdyne.com/) <br/> [support@trackdyne.com](mailto:support@trackdyne.com) | **AsterGrid** - underwater acoustic navigation system <br/> AsterGrid Nav Host software: User's manual |

# AsterGrid Nav Host software: <br/> User's manual

<div style="page-break-after: always;"></div>

## Contents

- [1. Introduction](#1-introduction)
- [2. Creating a Bluetooth connection with a PC](#2-creating-a-bluetooth-connection-with-a-pc)
- [3. Using the software](#3-using-the-software)

<div style="page-break-after: always;"></div>

## 1. Introduction
This manual describes the process of connecting the diver's navigation receiver [AsterGrid Nav](/documentation/EN/AsterGrid/AsterGrid_Nav_Specification_en.html) to a PC.
PC system requirements for connecting the device:
- **Windows 10** OS with **.NET Framework 4.5** installed

For earlier versions of the device, released before 2025, the following will be required:
- **Bluetooth** module

> CAUTION! To pair devices released later than January 2025, creating a Bluetooth connection with the PC is not required. Instead, connect the device to the PC using the supplied cable. In this case, installation of the USB-Serial converter driver may be required.

## 2. Creating a Bluetooth connection with a PC
The Bluetooth adapter on the PC must be turned on, and the diver's navigation receiver [AsterGrid Nav](/documentation/EN/AsterGrid/AsterGrid_Nav_Specification_en.html) must be placed on the charging pad connected to power.
Below is the sequence of steps for creating a Bluetooth connection, using a PC with Windows 10 installed as an example.

1. Open the menu **Start -> Settings -> Devices**
2. Make sure that the **Bluetooth** switch is in the **On** position
3. Press the **+ Add Bluetooth or other device** button

After the system detects a new device, it is displayed in the list, as in **Figure 1**.

<table>
<tbody>
<tr><td align="center" markdown="span">![Fig. 1](/documentation/astergrid_nav_bluetooth_pairing.png)</td></tr>
<tr><td align="center" markdown="span">**Figure 1 - Search results for new devices**</td></tr>
</tbody>
</table>

In **Figure 1**, the list shows the name of the device, which is visible on the screen of the device itself (in the example, **RDNV-4B8C**). Next, when the **Pair** button is pressed, the system prompts to enter a PIN code (shown in **Figure 2**).

<table>
<tbody>
<tr><td align="center" markdown="span">![Fig. 2](/documentation/astergrid_nav_bluetooth_pin.png)</td></tr>
<tr><td align="center" markdown="span">**Figure 2 - Dialog for entering a PIN code**</td></tr>
</tbody>
</table>

The PIN code that must be entered to establish a connection with the device is displayed on the device screen (**1945** in the example). Enter the PIN code and press the **Next** button.

Wait for the connection with the device to be established. After that, the dialog window should look as in **Figure 4**. Device status: **Connected**.

<table>
<tbody>
<tr><td align="center" markdown="span">![Fig. 4](/documentation/astergrid_nav_bluetooth_connected.png)</td></tr>
<tr><td align="center" markdown="span">**Figure 4 - Device is connected**</td></tr>
</tbody>
</table>

At this stage, the connection with the device is established.

## 3. Using the software
After connecting the device according to [section 2](#2-creating-a-bluetooth-connection-with-a-pc), you can launch the AsterGrid Nav configuration utility (available on request from [support@trackdyne.com](mailto:support@trackdyne.com)), and it will establish the connection with the device by itself. If the connection is successful, the status "connected" is displayed in the status bar of the application window. The device name appears in the window title (in the example, **RDNV-4B8C**).  

The upper lines display the device version information and its serial number. Below, the version information of the navigation receiver and its serial number are displayed. This information is available only if the device was switched to service mode from the powered-on state, rather than placed on the charging pad while switched off.

After connecting, the user can change the settings. The diver's navigation receiver has a minimum number of settings.
In particular, for correct operation only the water salinity needs to be set.

If work is planned in freshwater bodies, it is recommended to leave the default value - **0 PSU**. For convenience, the application contains a database of world ocean salinities for points with a step of **1˚** in latitude and longitude.

To look up the salinity of a water body, enter the geographic coordinates of the location in the dialog opened by the **Search in base** link of the application main window.

After entering the coordinates of the location (one-degree accuracy is sufficient) and pressing the **Search** button, the salinity value at the nearest known point with a measured salinity is displayed.

When the **OK** button is pressed, the found value is placed in the settings field of the main window.

Additionally, it is possible to configure flipping of the device screen with a simultaneous swap of the button functions. This function is intended to allow the device to be mounted on the right hand.
To enable this function, check the **Right-handed device** check box in the main application window.

To upload the settings to the device, press the **Save** button.
The **Download** button is used to download the track recorded by the device, the buoy positions and the saved points from the device.

After the **Download** button is pressed, the other buttons become unavailable while the track is being downloaded from the device, and the progress of the operation is displayed in the application status bar.

When the download is complete, the application offers to save the downloaded data using the standard system dialog. The proposed file name is composed of the current system time and date.
The application allows saving the track in **Keyhole Markup Language (KML)** format. The track can then be imported into mapping software (for example, Google Earth).

After the data is saved, the application asks the user whether to clear the track from the device.

> CAUTION! After the track is cleared from the device, it will be impossible to restore it. At all.

Working with waypoints is done using the context menu, opened with the right mouse button on the **Waypoints** group.

Manually added points can be edited using the panel that appears on the right when an added point is selected.

To synchronize the list in the **Waypoints** panel with the device, press the **Upload to device** button. To clear all waypoints in the device, delete them in the list, then press the **Upload to device** button and answer yes to the application's prompt.

<div style="page-break-after: always;"></div>

______________
[Back to contents](#contents)

<div style="page-break-after: always;"></div>
