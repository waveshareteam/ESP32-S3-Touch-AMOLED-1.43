# 04_SD_Card

[English](README.md) | [简体中文](README_ZH.md)

## What It Does

Mounts a microSD card and reports card information and capacity.

## Hardware Required

ESP32-S3-Touch-AMOLED-1.43 development board and a USB data cable. Insert a microSD card into the onboard slot before starting.

## How to Run

Open an ESP-IDF terminal in this directory and run with a version listed in the repository README:

```bash
idf.py set-target esp32s3 build flash monitor
```

## Expected Result

The log shows card information and capacity after a successful mount.

## Troubleshooting

The mount configuration enables formatting on mount failure; use a card whose contents are backed up.
