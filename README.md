Hardware Setup

Use these connections:

    CLK  D1
    DIN  D2
    DC  D5
    CE  D6
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
