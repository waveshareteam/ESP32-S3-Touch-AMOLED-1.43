# factory

[English](README.md) | [简体中文](README_ZH.md)

## What It Does

Runs the factory interface for display, touch, RTC, IMU, battery ADC, SD card, Wi-Fi/BLE scanning and button/GPIO tests.

## Hardware Required

ESP32-S3-Touch-AMOLED-1.43 development board and a USB data cable. A battery and microSD card are needed for their corresponding tests; the GPIO test requires the loopback wiring defined in `components/gpio_bsp/`.

## How to Run

Open an ESP-IDF terminal in this directory and run with **v5.1.4**:

```bash
idf.py set-target esp32s3 build flash monitor
```

## Expected Result

The touchscreen interface shows peripheral readings and test status; scan buttons list nearby wireless devices.

## Troubleshooting

Missing loopback wiring causes the GPIO test to report failure; the SD mount configuration can format the card on failure.
