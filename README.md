# Bluetooth-Enabled-Wireless-Notice-Board
This is a Bluetooth Enabled Wireless Notice Board, which uses the LPC2129 microcontroller, paired with a HD44780 16x2 Alphanumeric LCD (the notice board itself), along with the HC-05 Bluetooth module, connected to the Serial Bluetooth terminal app in the mobile phone, to send the required messages.

Testing Steps & Operation:

1. Power up the circuit. 
2. The LCD will display "Wireless Notice Board Ready...".
3. Open your smartphone's Bluetooth settings, search for HC-05, and pair using code 1234.
4. Open the Serial Bluetooth Terminal app (available on Android).
5. Connect to the HC-05 inside the app menu.
6. Type any message up to 16 characters (e.g., EXAM AT 2 PM) and hit Send.
7. The LPC2129 will instantly clear the old notice and write the new text onto the second line of the display.
