# 05_WIFI_AP

[English](README.md) | [简体中文](README_ZH.md)

## What It Does

Creates a 2.4 GHz Wi-Fi access point.

## Hardware Required

ESP32-S3-Touch-AMOLED-1.43 development board and a USB data cable. Use a phone or computer with Wi-Fi to find the access point.

## How to Run

Install the Arduino-ESP32 version listed in the repository README, set the sketchbook to `examples/arduino/`, then open and upload the matching `.ino`. Select **ESP32S3 Dev Module** and use **115200** in the serial monitor.

| Tools menu | Value |
| --- | --- |
| Flash Size | 16MB (128Mb) |
| Partition Scheme | 16M Flash (3MB APP/9.9MB FATFS) |
| PSRAM | OPI PSRAM |
| USB CDC On Boot | Enabled |

## Expected Result

The access point appears in the Wi-Fi network list and accepts client connections.

## Troubleshooting

The default SSID is `bsp_esp_demo` with password `waveshare`; edit the access-point settings in the source and upload again.
