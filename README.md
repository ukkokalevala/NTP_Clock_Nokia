Hardware Setup

Use these connections:

CLK  D1
DIN  D2
DC   D5
CE   D6
RST  D7

Software Requirements

For the Nokia 5110 display, you’ll need:

Adafruit_PCD8544 and Adafruit_GFX libraries.
NTPClient for time synchronization.
ESP8266WiFi for the Wemos D1 Mini.

Explanation of the Code

Wi-Fi Connection: Connects to Wi-Fi using the Wemos D1’s credentials.
Time and Date Display: The current time is displayed on the top of the Nokia 5110, and the date is displayed beneath it.

This code will update every second, showing the current network-synced time and date on your Nokia 5110 display.

Nokia LCD display 5110 configuration:
    
CLK (Clock) - 
D1: This is the SPI clock line. It synchronizes data transmission between the Wemos and the Nokia display.

DIN (Data In) - 
D2: This is the SPI MOSI (Master Out Slave In) line. The Wemos sends data to the display through this pin.

DC (Data/Command) - 
D5: This pin tells the display whether incoming data is a command (low) or display data (high).

CE (Chip Enable) - 
D6: Also known as Chip Select (CS). It activates the display for data transfer when pulled low.

RST (Reset) - 
D7: Resets the display when pulled low.

