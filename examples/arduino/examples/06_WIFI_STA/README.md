# 06_WIFI_STA

[English](README.md) | [简体中文](README_ZH.md)

## What It Does

Connects the board to a 2.4 GHz Wi-Fi access point in station mode.

## Hardware Required

ESP32-S3-Touch-AMOLED-1.43 development board and a USB data cable. A 2.4 GHz Wi-Fi access point is required.

## How to Run

Set the SSID and password in the example's Wi-Fi source before building.

Install the Arduino-ESP32 version listed in the repository README, set the sketchbook to `examples/arduino/`, then open and upload the matching `.ino`. Select **ESP32S3 Dev Module** and use **115200** in the serial monitor.

| Tools menu | Value |
| --- | --- |
| Flash Size | 16MB (128Mb) |
| Partition Scheme | 16M Flash (3MB APP/9.9MB FATFS) |
| PSRAM | OPI PSRAM |
| USB CDC On Boot | Enabled |

## Expected Result

The log prints an IP address when the connection succeeds.

## Troubleshooting

The supplied credentials are `bsp_esp_demo` / `waveshare`; they must match the access point.
