[Main](/) ❯ [Underwater acoustic modems](/underwater_acoustic_modems_en.html) ❯ **Vexa Mini: Firmware update guide**

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

| ![Trackdyne](/documentation/logo.svg) | |
| :---: | ---: |
| [trackdyne.com](https://trackdyne.com/) <br/> [support@trackdyne.com](mailto:support@trackdyne.com) | Firmware update guide for Vexa Mini modems  |

<div style="page-break-after: always;"></div>

# Updating the firmware of Vexa Mini modems

> We are constantly working to improve our products, taking into account the opinions and wishes of users and eliminating the shortcomings we find. You can find the version history, new features and bug fixes on the page [Vexa Mini: Version history & changes](/documentation/EN/Vexa/Vexa_version_history_en.html).

## Step 1
Download the necessary utilities.

### Step 1.1
Get the modem host application (available on request from [support@trackdyne.com](mailto:support@trackdyne.com)) to work with Vexa Mini modems. The application runs on a PC under Windows OS (version 8 or later).

### Step 1.2
Get the firmware update utility (available on request from [support@trackdyne.com](mailto:support@trackdyne.com)). The utility runs on a PC under Windows OS (version 8 or later).

### Step 1.3
Simply unpack the downloaded archives into folders of your choice. Neither application requires installation.

## Step 2
Prepare everything for connecting the modem to the PC.

### Step 2.1
Connect your modem to a **UART<->USB** converter. The wire assignment by color is shown below:  

<table>
<thead><tr><th align="center" markdown="span">![Vexa Mini_wiring_diagram_en](/documentation/Vexa_Mini_wiring_diagram_en.png)</th></tr></thead>
<tbody>
<tr><td align="center" markdown="span">Figure 1. Cable wire assignment</td></tr>
</tbody>
</table>

The voltage on the data lines **MUST NOT** exceed 3.3 V.
To switch the modem to command mode initially, provide a means of pulling the SVC/CMD wire up to a voltage of 3.3 or 5 V. This is conveniently done with a jumper.

### Step 2.2
Provide a convenient way of switching the command mode on and off, as shown in the diagrams below.

<table>
<thead><tr><th align="center" markdown="span">![vexa_mini_usb_cmd_mode_off](/documentation/vexa_mini_usb_cmd_mode_off.png)</th></tr></thead>
<tbody>
<tr><td align="center" markdown="span">Figure 2. Connecting the modem to the PC USB port using an interface converter. **Command mode off**</td></tr>
</tbody>
</table>

<table>
<thead><tr><th align="center" markdown="span">![vexa_mini_usb_cmd_mode_on](/documentation/vexa_mini_usb_cmd_mode_on.png)</th></tr></thead>
<tbody>
<tr><td align="center" markdown="span">Figure 3. Connecting the modem to the PC USB port using an interface converter. **Command mode on**</td></tr>
</tbody>
</table>

## Step 3
Connect the device to the PC USB port.

### Step 3.1
Make sure that the command mode is not enabled (the jumper is removed, the **SVC/CMD** wire is pulled to ground - as shown in the diagram in Fig. 2)

### Step 3.2
Connect the modem to the PC USB port using the converter:

<table>
<thead><tr><th align="center" markdown="span">![vexa_mini_and_uart_usb_converter3](/documentation/vexa_mini_and_uart_usb_converter3.png)</th></tr></thead>
<tbody>
<tr><td align="center" markdown="span">Figure 4. The modem is connected to the PC</td></tr>
</tbody>
</table>

## Step 4
Enable the **Command mode by default** setting.

### Step 4.1
Launch the modem host application (available on request from [support@trackdyne.com](mailto:support@trackdyne.com))

### Step 4.2
Press the **SETTINGS** button on the top toolbar.

### Step 4.3
In the settings window that opens, select the required port and press the **OK** button.

### Step 4.4
The application will prompt you to restart it to apply the new settings - confirm by pressing the **OK** button.

### Step 4.5
After the application restarts, press the **CONNECT** button.
If the application has successfully opened the port, the **CONNECT** button will become highlighted and change its name to **DISCONNECT**, and a corresponding message will be displayed in the **HISTORY WINDOW** text box.

If any error occurs, make sure that the port has been selected correctly and, if necessary, return to [Step 4.2](#step-42).

### Step 4.6
Press the **COMMAND MODE** button, thereby informing the application that you are going to work with the modem in command mode.

### Step 4.7
Put the modem into command mode by pulling the **SVC/CMD** wire up to 3.3 or 5 V.

### Step 4.8
Press the **QUERY** button on the **DEVICE INFO** tab. If everything is done correctly, the corresponding information will be displayed in the **HISTORY WINDOW** and in the text field on the **DEVICE INFO** tab.

Make sure that the **Command mode by default** checkbox is checked. If it is not, check it and press the **APPLY** button to change the modem settings.

If this does not happen, close the port by pressing the **DISCONNECT** button and go to [Step 4.2](#step-42). If the port is selected correctly after all, make sure that the **SVC/CMD** wire was pulled to "ground" at the moment power was applied to the modem, i.e. go to [Step 3](#step-3).

### Step 4.9
Close the modem host application (available on request from [support@trackdyne.com](mailto:support@trackdyne.com))

### Step 4.10
Pull the **SVC/CMD** wire to "ground".

## Step 5
Updating the device firmware

### Step 5.1
If you do not have a firmware file for this modem, contact [technical support](mailto:support@trackdyne.com) to obtain the firmware file. In the e-mail, state the serial number of the device:

### Step 5.2
Launch the firmware update utility (available on request from [support@trackdyne.com](mailto:support@trackdyne.com)).

### Step 5.3
Connect the modem to the PC via the interface converter, as shown in [Step 3](#step-3), making sure before connecting that the **SVC/CMD** wire is pulled to "ground".

### Step 5.4
In the **Port** drop-down list, select the port corresponding to the device.

### Step 5.5
Select the firmware file corresponding to the device by pressing the **Load** button.

### Step 5.6
Start the firmware update process by pressing the **Start** button.

If:  
* the port is selected correctly
* the firmware file corresponds to the serial number of the device
* before power was applied to the device, the **SVC/CMD** wire was pulled to ground

Then the progress of the firmware update will start to be displayed in the bottom text field.

### Step 5.7
Close the application and disconnect the modem from the PC. The update is complete.

If the device firmware update cannot be performed, check the following possible causes:

* the port was selected incorrectly
* the firmware file does not correspond to the serial number of the device
* before power was applied to the device, the **SVC/CMD** wire was not pulled to ground
* the connection was interrupted during the firmware update

If the update cannot be performed, [contact technical support](mailto:support@trackdyne.com).

<div style="page-break-after: always;"></div>
