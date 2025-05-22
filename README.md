# ESP32 Internet Radio with Display and Audio Amplifier

# 1.Description
This project is an Internet Radio built using an ESP32 microcontroller. It streams audio from internet radio stations, displays station and playback info on an OLED screen, and outputs sound through a PAM8403 audio amplifier and speaker. A rotary encoder is used for volume or station control.

# 2.Components Used
- ESP32 Development Board
- OLED Display (SSD1306, I2C)
- PAM8403 Audio Amplifier Module
- Speaker
- Rotary Encoder with Push Button
- 5V Power Supply
- Connecting wires

# 3.How It Works
- The *ESP32* connects to Wi-Fi and streams audio from internet radio stations.
- The *OLED display* shows the current station, bitrate, and connection status.
- The *rotary encoder* is used to switch between stations or adjust volume.
- The *PAM8403 amplifier* boosts the audio signal and drives the speaker.
- The *speaker* plays the audio streamed through ESP32.

# 4.Wiring Summary

| Component            | ESP32 Pin |
|----------------------|-----------|
| OLED SDA             | 1021      |
| OLED SDK             | 1024      |
| Rotary Encoder CLK   | D33       |
| Rotary Encoder DT    | D32       |
| Rotary Encoder SW    | D25       |
| PAM8403 L/R IN       | Audio Out from ESP32 (e.g., DAC1/DAC2) |
| PAM8403 VCC          | 5V        |
| PAM8403 GND          | GND       |
| Speaker              | Output from PAM8403 |

> ## *Note:* Exact DAC pins for audio output can vary. Common options: GPIO25 (DAC1), GPIO26 (DAC2).

# 4.Libraries Required(Arduino)
- WiFi.h
- ESPAsyncWebServer.h
- ESP32-audioI2S
- Adafruit_SSD1306
- RotaryEncoder

# 5.Photos
(https://github.com/Akez76/Arduino-Internet-radio/blob/main/Arduino%20Wifi2.jpeg)
(https://github.com/Akez76/Arduino-Internet-radio/blob/main/Arduino%20Wifi1.jpeg)
(https://github.com/Akez76

# 6.Skills Used / Learned
- Internet audio streaming
- Rotary encoder integration
- OLED graphics with I2C
- Amplifier & speaker output
- ESP32 Wi-Fi & real-time audio

# Author:
Akezhan Kurbanov
