# Bluetooth-Enabled-Wireless-Notice-Board
This is a Bluetooth Enabled Wireless Notice Board, which uses the LPC2129 microcontroller, paired with a HD44780 16x2 Alphanumeric LCD (the notice board itself), along with the HC-05 Bluetooth module, connected to the Serial Bluetooth terminal app in the mobile phone, to send the required messages.

Components Needed:
1. LPC2129 Microcontroller
2. HD44780 16x2 Alphanumeric LCD
3. HC-05 Bluetooth module
4. Smartphone with Serial Bluetooth terminal app installed
5. Connecting wires as required

Testing Steps & Operation:

1. Power up the circuit. 
2. The LCD will display "Wireless Notice Board Ready".
3. Open your smartphone's Bluetooth settings, search for HC-05, and pair using code 1234.
4. Open the Serial Bluetooth Terminal app (available on Android).
5. Connect to the HC-05 inside the app menu.
6. Type any message up to 32 characters (it moves to the second line of the 16x2 LCD automatically) (e.g., EXAM AT 2 PM) and hit Send.
7. The LPC2129 will instantly clear the old notice and write the new text onto the second line of the display.
