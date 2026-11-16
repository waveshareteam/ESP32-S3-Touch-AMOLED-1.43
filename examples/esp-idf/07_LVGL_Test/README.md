# 07_LVGL_Test

[English](README.md) | [简体中文](README_ZH.md)

## What It Does

Runs the LVGL widgets demonstration on the onboard AMOLED display with capacitive touch input.

## Hardware Required

ESP32-S3-Touch-AMOLED-1.43 development board and a USB data cable.

## How to Run

Open an ESP-IDF terminal in this directory and run with a version listed in the repository README:

```bash
idf.py set-target esp32s3 build flash monitor
```

## Expected Result

The display shows interactive LVGL widgets that respond to touch.

## Troubleshooting

This example uses LVGL 8 APIs; do not replace its dependency with LVGL 9.
