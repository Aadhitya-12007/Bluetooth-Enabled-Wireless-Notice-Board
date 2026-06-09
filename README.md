# Bluetooth-Enabled Wireless Notice Board

![Hardware](https://img.shields.io/badge/Hardware-LPC2129-blue.svg)
![Connectivity](https://img.shields.io/badge/Connectivity-Bluetooth_HC--05-0082FC.svg)
![Display](https://img.shields.io/badge/Display-16x2_LCD-brightgreen.svg)

A smart, wireless digital notice board powered by the **NXP LPC2129 (ARM7) microcontroller**. This project allows users to instantly update physical display boards wirelessly from their smartphones using an HC-05 Bluetooth module and a standard 16x2 Alphanumeric LCD. 

Perfect for classrooms, offices, or labs where dynamic, real-time information needs to be displayed without the hassle of cables.

## Key Features

* Send messages instantly from any Bluetooth-enabled smartphone.
* Supports messages up to 32 characters, automatically wrapping text from the first line to the second line of the 16x2 LCD.
* Works with standard Serial Bluetooth Terminal applications (no custom app required).
* Clears the old notice and seamlessly displays the new one upon receiving a transmission.

## Hardware Requirements

To replicate this project, you will need the following components:

* 1x **LPC2129 Microcontroller** (ARM7TDMI-S based)
* 1x **HD44780 16x2 Alphanumeric LCD** (The notice board display)
* 1x **HC-05 Bluetooth Module** (For wireless communication)
* 1x **Android Smartphone** (For sending data)
* Connecting jumper wires and a breadboard/PCB

## 📲 Software Requirements

* **[Serial Bluetooth Terminal](https://play.google.com/store/apps/details?id=de.kai_morich.serial_bluetooth_terminal)** (or any similar Bluetooth terminal app available on Android/iOS).

## Testing Steps & Operation

Follow these steps to set up and use the wireless notice board:

1. Supply power to the microcontroller circuit. 
2. Upon successful boot, the LCD will display the welcome message:  
   > `"Wireless Notice Board Ready"`
3. For the bluetooth pairing:
   * Open your smartphone's Bluetooth settings.
   * Search for available devices and select the **HC-05** module.
   * Pair the device using the default PIN code: **`1234`** (or `0000`). *NOTE:* This depends on the type of bluetooth sensor, generally it is 1234 by default.
5. Open the Serial Bluetooth Terminal app on your phone.
6. Inside the app menu, connect to your paired HC-05 module.
7. Type your desired message (up to 32 characters). 
   * *Example:* `EXAM AT 2 PM`
   * Hit **Send**.
8. The LPC2129 MCU will instantly clear the old notice and write your new text onto the display, utilizing the second line automatically if the text exceeds 16 characters.

## Contributing

Contributions, issues, and feature requests are welcome!
