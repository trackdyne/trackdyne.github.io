[Main](/) ❯ [Underwater acoustic modems](/underwater_acoustic_modems_en) ❯ **Instructions for firmware updating: Vexa family**

<div style="page-break-after: always;"></div>

| ![Trackdyne](/documentation/logo.svg) | |
| :---: | ---: |
| [trackdyne.com](https://trackdyne.com/) <br/> [support@trackdyne.com](mailto:support@trackdyne.com) | Instructions for updating the firmware of Vexa Mini modems   |

<div style="page-break-after: always;"></div>

# Updating the firmware of Vexa Mini modems

>We are constantly working to improve products, take into account the opinions and wishes of users and eliminate the identified shortcomings. Version history, new feature additions, and bug fixes can be found on the [Vexa Mini: Version and Changes History](Vexa_version_history_en.md) page.

## Step 1 
Download the necessary utilities.

### Step 1.1 
Get the modem host application (available on request from [support@trackdyne.com](mailto:support@trackdyne.com)) to work with Vexa Mini modems. The application runs on a PC running Windows OS (Version 8 and above).

### Step 1.2 
Get the firmware update utility (available on request from [support@trackdyne.com](mailto:support@trackdyne.com)). The utility works on a PC running OC Windows (Version 8 and higher).

### Step 1.3 
Just unpack the downloaded archives into folders convenient for you. Both applications do not require installation.

## Step 2
Prepare everything to connect the modem to the PC.

### Step 2.1 
Connect your modem to the **UART<->USB** converter. The purpose of the cable cores by color is shown below:

<table>
<thead><tr><th align="center" markdown="span">![Vexa Mini_wiring_diagram_en](/documentation/Vexa_Mini_wiring_diagram_en.png)</th></tr></thead>
<tbody>
<tr><td align="center" markdown="span">Fig 1. Functions of cable cores</td></tr>
</tbody>
</table>

The voltage on the data lines **MUST NOT** exceed 3.3 V.
For the initial switching of the modem to the command mode, it is necessary to provide for the possibility of tightening the SVC / CMD wire to a voltage of 3.3 or 5 Volts. It is convenient to do this with a jumper.

### Step 2.2 
Provide the ability to conveniently turn on and off the command mode according to the diagrams below.

<table>
<thead><tr><th align="center" markdown="span">![vexa_mini_usb_cmd_mode_off](/documentation/vexa_mini_usb_cmd_mode_off.png)</th></tr></thead>
<tbody>
<tr><td align="center" markdown="span">Fig 2. Connecting a modem to a PC USB port using an interface converter. **Command mode OFF**</td></tr>
</tbody>
</table>

<table>
<thead><tr><th align="center" markdown="span">![vexa_mini_usb_cmd_mode_on](/documentation/vexa_mini_usb_cmd_mode_on.png)</th></tr></thead>
<tbody>
<tr><td align="center" markdown="span">Fig 3. Connecting a modem to a PC USB port using an interface converter. **Command mode ON**</td></tr>
</tbody>
</table>


## Step 3
Connecting the device to the USB port of the PC.

### Step 3.1 
Make sure that the command mode is not enabled (jumper removed, **SVC/CMD** wire pulled to GND- as shown in the diagram in Fig. 2).

### Step 3.2 
Connect the modem to the USB port of the PC using a converter:

<table>
<thead><tr><th align="center" markdown="span">![vexa_mini_and_uart_usb_converter3](/documentation/vexa_mini_and_uart_usb_converter3.png)</th></tr></thead>
<tbody>
<tr><td align="center" markdown="span">Fig 4. Modem is connected to a PC</td></tr>
</tbody>
</table>

## Step 4
Enabling the **Command mode by default** setting.

### Step 4.1 
Start the modem host application.

### Step 4.2 
Press the **SETTINGS** button on the top toolbar.

### Step 4.3 
In the settings window that opens, select the desired port and click the **OK** button.

### Step 4.4
The application will prompt to restart it to apply the new settings - confirm by pressing the **OK** button.

### Step 4.5 
After restarting the application, press the **CONNECT** button.
If the application was able to successfully open the port, the **CONNECT** button will become highlighted and change its name to **DISCONNECT** and a corresponding message will be displayed in the **HISTORY WINDOW** text box.

If any error occurs, check that the correct port has been selected and return to [Step 4.2](#step-42) if necessary.

### Step 4.6
Press the **COMMAND MODE** button, thereby informing the application that you are going to work with the modem in command mode.

### Step 4.7
Put the modem into command mode by pulling the **SVC/CMD** wire to 3.3 or 5 Volts.

### Step 4.8
Press the **QUERY** button on the **DEVICE INFO** tab. If everything is done correctly, then in the **HISTORY WINDOW** windows and the text field on the **DEVICE INFO** tab, the corresponding information will be displayed.

Make sure the **Command mode by default** checkbox is checked. If not, install it and press the **APPLY** button to change the modem settings.

If it doesn't, close the port by pressing the **DISCONNECT** button and go to [Step 4.2](#step-42). If the port is selected correctly, make sure that the **SVC/CMD** wire was pulled to GND when power was supplied to the modem, i.e. go to [Step 3](#step-3).

### Step 4.9
Close modem host application.

### Step 4.10
Pull the **SVC/CMD** conductor to the GND.

## Step 5
Updating device firmware

### Step 5.1
If you do not have a firmware file for this modem, please contact the [developer](mailto:support@trackdyne.com) for a firmware file. In the letter, place the serial number of the device:

### Step 5.2
Start the firmware update utility.

### Step 5.3
Connect the modem to the PC via the interface converter as shown in [Step 3](#step-3), making sure the **SVC/CMD** wire is pulled to GND before connecting.

### Step 5.4
In the **Port** Combobox, select the appropriate port for the device.

### Step 5.5
Select the appropriate firmware file for the device by pressing the **Load** button.

### Step 5.6
Start the firmware update process by pressing the **Start** button.

If:
* port is correct
* the firmware file corresponds to the serial number of the device
* before powering up the device, the **SVC/CMD** wire was pulled to the GND

Then, the bottom text box will start to display the progress of the firmware update.

### Step 5.7
Close the application and disconnect the modem from the PC. Update completed.

If the device firmware update fails, check the following reasons:

* port selected incorrectly
* the firmware file does not match the serial number of the device
* before powering up the device, the **SVC/CMD** wire was not connected to GND
* the connection was broken during the firmware update

If the update fails, [contact the developer](mailto:support@trackdyne.com)

<div style="page-break-after: always;"></div>
