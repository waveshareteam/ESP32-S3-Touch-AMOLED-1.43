# 08_LVGL_SDIMG

[English](README.md) | [简体中文](README_ZH.md)

## What It Does

Lists images on a microSD card and displays the selected image through LVGL.

## Hardware Required

ESP32-S3-Touch-AMOLED-1.43 development board and a USB data cable. A microSD card with a `Test` folder in its root is required.

## How to Run

Copy the pictures in `Test_IMG_SRC/` into the card's `Test/` folder before starting.

Open an ESP-IDF terminal in this directory and run with a version listed in the repository README:

```bash
idf.py set-target esp32s3 build flash monitor
```

## Expected Result

Use the touchscreen to scan the folder and select an image to display.

## Troubleshooting

The browser lists at most 20 entries; use the supplied BMP, JPG and PNG samples. Mount failure may format the card.
