# 06_WIFI_STA

[English](README.md) | [简体中文](README_ZH.md)

## What It Does

Connects the board to a 2.4 GHz Wi-Fi access point in station mode.

## Hardware Required

ESP32-S3-Touch-AMOLED-1.43 development board and a USB data cable. A 2.4 GHz Wi-Fi access point is required.

## How to Run

Set the SSID and password in the example's Wi-Fi source before building.

Open an ESP-IDF terminal in this directory and run with a version listed in the repository README:

```bash
idf.py set-target esp32s3 build flash monitor
```

## Expected Result

The log prints an IP address when the connection succeeds.

## Troubleshooting

The supplied credentials are `bsp_esp_demo` / `waveshare`; they must match the access point.
